---
title: Тип ресурса report
description: Описывает ресурс отчета API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: f94be1bcc5dfde092c6360bbdddd96d604d30a55
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939674"
---
# <a name="report-resource-type"></a>Тип ресурса report

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возвращает содержимое, подходящее для контекста, в том числе:

- Отчеты об истории профилей конфигурации устройств.
- Отчеты о сбоях регистрации.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|содержимое|Поток|Содержимое отчета; сведения зависят от типа отчета.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.report"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.report",
  "content": "<Unknown Primitive Type Edm.Stream>"
}
```



