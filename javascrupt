function askAI() {
    const input = document.getElementById('userInput').value.trim();
    const responseDiv = document.getElementById('response');
  
    if (!input) {
      responseDiv.textContent = "隢见��撓�亙�誯���䈑�";
      return;
    }
  
    const responses = [
      {
        keywords: ["憭拇除", "瘞�澈", "瘞�情"],
        replies: ["隞𠰴予�荗��� ��儭�", "��厰�鮋苊嚗䔶�銝齿�銝钅𢂚 ��儭�", "�虾�賣���匧���屸𡺨�腼�𢂚 ����𧶏��枂��隢见葆�矋�"]
      },
      {
        keywords: ["雿䭾糓隤�", "雿惩㙈隞�暻�", "雿䭾糓隞�暻�"],
        replies: ["��烐糓雿删� AI 撠誩鼠��页��鴂�", "��𤏸◤閮剛���撟怠𨭌雿㰘圾瘙箏�誯�䕘��", "��煾�𣇉�嗡�齿糓鈭粹�痹�䔶���穃����誩鼠雿� ��働"]
      },
      {
        keywords: ["�����", "撟暸��", "�𣶹�銁"],
        replies: [() => `�𣶹�銁����𤘪糓 ${new Date().toLocaleTimeString()}`]
      },
      {
        keywords: ["�滩��", "�緵�緵", "bye"],
        replies: ["�緵�緵嚚䂿�苷�䭾�厩�𤾸末��銝�憭抬�����", "銝𧢲活�滩�见�㚁��", "��烐��喃�删� ����"]
      }
    ];
  
    // 瑼Ｘ䰻雿輻鍂��頛詨�亦泵���𪑛�见�墧�㗇�苷辣
    let found = false;
    for (const group of responses) {
      for (const keyword of group.keywords) {
        if (input.includes(keyword)) {
          const reply = group.replies[Math.floor(Math.random() * group.replies.length)];
          responseDiv.textContent = typeof reply === "function" ? reply() : reply;
          found = true;
          break;
        }
      }
      if (found) break;
    }
  
    if (!found) {
      // �𨯬�鍂��墧��
      const defaultReplies = [
        "�䠷�峕�煾���銁摮貊�雴葉嚗峕�𥕦�𧢲䲮撘誩�讐�讠�页�跔鴂�",
        "��睲�滚云��雿惩銁��譍�暻潸�塚�諹�質牧敺埈凒皜�璆𡁜�𠬍��",
        "�坔�誯�峕�厰�噼���頣�䔶�𧢲活��烐��𠜱��𥕦飛���� ����"
      ];
      responseDiv.textContent = defaultReplies[Math.floor(Math.random() * defaultReplies.length)];
    }
  }
