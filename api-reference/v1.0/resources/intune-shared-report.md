---
title: Тип ресурса report
description: Отчет, который изменяется в зависимости от рабочего процесса, либо устройства профиля конфигурации журнала или регистрации ошибок.
localization_priority: Normal
ms.openlocfilehash: 8854bb0f32c1360a4c529137a3f587f7a3cba5f2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862162"
---
# <a name="report-resource-type"></a>Тип ресурса report

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.


Отчет, который изменяется в зависимости от рабочего процесса, либо устройства профиля конфигурации журнала или регистрации ошибок.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|content|Stream|Н/Д|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.report"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.report",
  "content": "<Unknown Primitive Type Edm.Stream>"
}
```
