---
title: тип перечисления Полицисетстатус
description: Перечисление, указывающее состояние набора политик.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 32ea9586ffee2ef112c58a1f88bdbdaefd654a04
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735164"
---
# <a name="policysetstatus-enum-type"></a>тип перечисления Полицисетстатус

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Перечисление, указывающее состояние набора политик.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|нуль|Значение по умолчанию.|
|нарушение|1,1|Все элементы набора политик теперь проверяют соответствующие параметры рабочих нагрузок.|
|партиалсукцесс|2|POST завершен для всех элементов с политиками, но существуют ошибки.|
|success|4|Все элементы с развернутыми политиками. Не означает, что развертывание завершено успешно. |
|error|4 |Обработка подполитики завершена с ошибками.|
|нотассигнед|5 |Policy/Полицисетитем не назначено ни одной группе.|





