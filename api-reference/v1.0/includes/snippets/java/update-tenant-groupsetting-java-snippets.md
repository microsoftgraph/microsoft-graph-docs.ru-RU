---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d35ef68fbbe64282b4dd8899dc7b5e9e7f4b9144
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394630"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupSetting groupSetting = new GroupSetting();
LinkedList<SettingValue> valuesList = new LinkedList<SettingValue>();
SettingValue values = new SettingValue();
values.name = "AllowToAddGuests";
values.value = "false";
valuesList.add(values);
groupSetting.values = valuesList;

graphClient.groupSettings("84af2ca5-c274-41bf-86e4-6e374ec4def6")
    .buildRequest()
    .patch(groupSetting);

```