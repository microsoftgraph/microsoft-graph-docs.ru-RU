---
title: Тип ресурса permissionGrantPolicy
description: Указывает условия, при которых может быть предоставлено согласие.
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 0d7868c3f0316703a62536a610ea29f2df9f13e7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117888"
---
# <a name="permissiongrantpolicy-resource-type"></a>Тип ресурса permissionGrantPolicy

Пространство имен: microsoft.graph

Политика предоставления разрешений используется для определения условий, при которых может предоставляться согласие.

Политика предоставления разрешений состоит из списка наборов условий **includes** и наборов условий **excludes**. Чтобы событие соответствовало политике предоставления разрешений, оно должно соответствовать *по крайней мере одному* набору условий **includes** и не должно соответствовать *никаким* наборам условий **excludes**.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Перечисление политик предоставления разрешений](../api/permissiongrantpolicy-list.md) | Коллекция [permissionGrantPolicy](permissiongrantpolicy.md) | Получение списка объектов permissionGrantPolicy. |
|[Создание политики предоставления разрешений](../api/permissiongrantpolicy-post-permissiongrantpolicies.md)| [permissionGrantPolicy](permissiongrantpolicy.md) | Создает новый объект permissionGrantPolicy. |
|[Получение политики предоставления разрешений](../api/permissiongrantpolicy-get.md) | [permissionGrantPolicy](permissiongrantpolicy.md) |Чтение свойств и связей объекта permissionGrantPolicy.|
|[Обновление политики предоставления разрешений](../api/permissiongrantpolicy-update.md) | [permissionGrantPolicy](permissiongrantpolicy.md)  |Обновление объекта permissionGrantPolicy. |
|**Наборы условий include**| | |
|[Перечисление наборов условий include](../api/permissiongrantpolicy-list-includes.md) |Коллекция [permissionGrantConditionSet](permissiongrantconditionset.md)| Получение наборов условий, *включенных* в политику предоставления разрешений.|
|[Добавление набора условий include](../api/permissiongrantpolicy-post-includes.md) |[permissionGrantConditionSet](permissiongrantconditionset.md) | Добавление набора условий, *включенного* из политики предоставления разрешений. |
|[Удаление набора условий include](../api/permissiongrantpolicy-delete-includes.md) | Нет | Удаление набора условий, *исключенного* из политики предоставления разрешений.|
|**Наборы условий exclude**| | |
|[Перечисление наборов условий exclude](../api/permissiongrantpolicy-list-excludes.md) |Коллекция [permissionGrantConditionSet](permissiongrantconditionset.md)| Получение наборов условий, *исключенных* в политике предоставления разрешений.|
|[Добавление набора условий exclude](../api/permissiongrantpolicy-post-excludes.md) |[permissionGrantConditionSet](permissiongrantconditionset.md) | Добавление набора условий, *исключенного* из политики предоставления разрешений. |
|[Удаление наборов условий exclude](../api/permissiongrantpolicy-delete-excludes.md) | Нет | Удаление набора условий, *исключенного* из политики предоставления разрешений.|

## <a name="properties"></a>Свойства

| Свойство     | Тип |Описание|
|:---------------|:--------|:----------|
| id | String | Уникальный идентификатор политики предоставления разрешений. Префикс **id** `microsoft-` зарезервирован для встроенных политик предоставления разрешений и не может использоваться в настраиваемой политике предоставления разрешений. Разрешены только буквы, числа, дефисы (`-`) и символы подчеркивания (`_`). Ключ. Значение null не допускается. Требуется при создании. Неизменяемый. |
| displayName | String |Отображаемое имя политики предоставления разрешений.|
| description |String| Описание политики предоставления разрешений.|
| includes | Коллекция [permissionGrantConditionSet](permissiongrantconditionset.md)| Наборы условий, *включенные* в эту политику предоставления разрешений. Автоматически расширяется в `GET`.|
| excludes |Коллекция [permissionGrantConditionSet](permissiongrantconditionset.md)| Наборы условий, *исключенные* в этой политике предоставления разрешений. Автоматически расширяется в `GET`.|

## <a name="relationships"></a>Связи

| Связь | Тип |Описание|
|:---------------|:--------|:----------|
|includes|Коллекция [permissionGrantConditionSet](permissiongrantconditionset.md)| Наборы условий, *включенные* в эту политику предоставления разрешений. Эта навигация автоматически расширяется в методе GET. |
|excludes|Коллекция [permissionGrantConditionSet](permissiongrantconditionset.md)| Наборы условий, *исключенные* в этой политике предоставления разрешений. Эта навигация автоматически расширяется в методе GET. |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.permissionGrantPolicy"
}-->

```json
{
  "id": "string (identifier)",
  "displayName": "string",
  "description": "string",
  "includes": "collection(microsoft.graph.permissionGrantConditionSet)",
  "excludes": "collection(microsoft.graph.permissionGrantConditionSet)"
}
```
