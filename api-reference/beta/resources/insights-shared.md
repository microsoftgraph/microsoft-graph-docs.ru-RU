---
title: тип общего ресурса
description: 'Возможность получения, представляющих файлы совместно с помощью или отдельного пользователя. Поддерживаются следующие общие файлы:'
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 289523f836d7b8080f7317e4d11301c71314ba93
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880614"
---
# <a name="shared-resource-type"></a>тип общего ресурса

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Возможность получения, представляющих файлы совместно с помощью или отдельного пользователя. Поддерживаются следующие общие файлы:

- Приглашение файлами, вложенными непосредственно в сообщение электронной почты или встрече.
- OneDrive для Bussiness и SharePoint современных вложения - файлов, хранящихся в OneDrive для бизнеса и SharePoint, которые пользователи совместно использовать как ссылки в сообщении электронной почты.

**Примечание**: Корпорация Майкрософт в настоящее время работает на заполнение результатов API совместно с данными. Возможно, некоторые данные, отсутствующие в первой недели после выпуска.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список общих](../api/insights-list-shared.md) |[insights_shared](insights-shared.md) коллекции| Получите список общих файлов.|

## <a name="properties"></a>Свойства

| Свойство              | Тип                      | Описание  |
| -------------         |---------------            | -------------|
| id                    | Строка                    | Уникальный идентификатор связи. Только для чтения.        |
| lastShared            | [sharingDetail](insights-sharingdetail.md)                | Сведения об общих элементов. Только для чтения.        |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | Свойства, которые можно использовать для визуализации документа в работу. Только для чтения      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | Свойства ссылки общих документов, таких как URL-адрес и тип документа. Только для чтения       |

## <a name="relationships"></a>Связи

| Свойство      | Тип          | Описание  |
| ------------- |---------------| -------------|
| resource      | Entity        | Используется для перехода к элементу, предоставлен общий доступ. Для файлов вложений тип — *fileAttachment*. Для связанного вложения тип — *driveItem*. |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
