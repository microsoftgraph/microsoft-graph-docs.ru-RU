---
title: Тип ресурса report
description: Отчет, который изменяется в зависимости от рабочего процесса, либо устройства профиля конфигурации журнала или регистрации ошибок.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 5945343684aa20dc8af403eb094bb29648ff4f8f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970236"
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
