---
title: тип enum defenderThreatAction
description: Действие защитника по умолчанию для решения обнаруженных угроз вредоносных программ.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a29ca5d0016c90d49ac6cc8febdf21b95feafef6
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60454602"
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
|userDefined|5|Разрешить пользователю определять действия, которые необходимо принять с обнаруженной угрозой.|
|block|6 |Заблокировать обнаруженную угрозу.|



