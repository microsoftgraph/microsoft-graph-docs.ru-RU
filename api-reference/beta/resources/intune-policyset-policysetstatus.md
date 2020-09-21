---
title: тип перечисления Полицисетстатус
description: Перечисление, указывающее состояние набора политик.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 71158908a14c2f621785b8b82cff480ea80cf92e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993373"
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
|нарушение|1 |Все элементы набора политик теперь проверяют соответствующие параметры рабочих нагрузок.|
|партиалсукцесс|2 |POST завершен для всех элементов с политиками, но существуют ошибки.|
|success|4|Все элементы с развернутыми политиками. Не означает, что развертывание завершено успешно. |
|error|4 |Обработка подполитики завершена с ошибками.|
|нотассигнед|5 |Policy/Полицисетитем не назначено ни одной группе.|






