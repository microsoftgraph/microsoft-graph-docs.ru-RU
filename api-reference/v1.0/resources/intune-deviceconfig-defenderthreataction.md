---
title: тип enum defenderThreatAction
description: Действие защитника по умолчанию для решения обнаруженных угроз вредоносных программ.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 636d20b3c71b62157946e77230cd8945dd9957cd
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758892"
---
# <a name="defenderthreataction-enum-type"></a>тип enum defenderThreatAction

Пространство имен: microsoft.graph

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




