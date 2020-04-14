---
title: тип перечисления Полицисетстатус
description: Перечисление, указывающее состояние набора политик.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b4fc37dd889edaa5a5050db3c162ec147d2573cf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448033"
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



