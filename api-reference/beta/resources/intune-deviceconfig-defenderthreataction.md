---
title: тип enum defenderThreatAction
description: Действие защитника по умолчанию для решения обнаруженных угроз вредоносных программ.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f533b3f9d751d52523c1fc2cb316604fa40827dc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59120229"
---
# <a name="defenderthreataction-enum-type"></a>тип enum defenderThreatAction

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Действие защитника по умолчанию для решения обнаруженных угроз вредоносных программ.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|deviceDefault|0|Применение действий на основе определения обновления.|
|очистка|1|Очистите обнаруженную угрозу.|
|карантин|2|Карантин обнаруженной угрозы.|
|удаление|3|Удалите обнаруженную угрозу.|
|разрешить|4 |Разрешить обнаруженную угрозу.|
|userDefined|5 |Разрешить пользователю определять действия, которые необходимо принять с обнаруженной угрозой.|
|block|6 |Заблокировать обнаруженную угрозу.|



