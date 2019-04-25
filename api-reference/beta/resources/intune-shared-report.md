---
title: Тип ресурса report
description: Описывает ресурс отчета API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: f523f6df0b8b90cb6649ac81f1e433d6df227aea
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534817"
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

## <a name="relationships"></a>Отношения
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



