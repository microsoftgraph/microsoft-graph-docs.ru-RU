---
title: Тип ресурса report
description: 'Отчет, который изменяется в зависимости от рабочего процесса: истории профиля конфигурации устройства или сбоев регистрации.'
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: ad95fa9ef21a6fbf80ddd8265b5bac2e72c1825b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253563"
---
# <a name="report-resource-type"></a>Тип ресурса report

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Отчет, который изменяется в зависимости от рабочего процесса: истории профиля конфигурации устройства или сбоев регистрации.

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
