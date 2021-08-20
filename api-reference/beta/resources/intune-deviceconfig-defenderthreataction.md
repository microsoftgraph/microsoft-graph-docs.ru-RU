---
title: тип enum defenderThreatAction
description: Действие защитника по умолчанию для решения обнаруженных угроз вредоносных программ.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3026c49e54ced17b3442458df20a15044123a25fc1dda23f303624ce49816093
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54243001"
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
|очистка|1 |Очистите обнаруженную угрозу.|
|карантин|2|Карантин обнаруженной угрозы.|
|удаление|3 |Удалите обнаруженную угрозу.|
|разрешить|4 |Разрешить обнаруженную угрозу.|
|userDefined|5 |Разрешить пользователю определять действия, которые необходимо принять с обнаруженной угрозой.|
|block|6 |Заблокировать обнаруженную угрозу.|




