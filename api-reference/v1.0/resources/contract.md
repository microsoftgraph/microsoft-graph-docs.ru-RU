---
title: Тип ресурса контракта
description: Представляет существующее партнерство, которое клиент-партнер имеет с клиентом-клиентом.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 2ec65433edf3a6d0ec5973c0a3bc8cf46cef00d0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962471"
---
# <a name="contract-resource-type"></a>Тип ресурса контракта

Пространство имен: microsoft.graph представляет существующее партнерство, которое клиент-партнер имеет с клиентом-клиентом.

> **Важно:** Существует только в клиентах-партнерах. Клиенты-партнеры — это клиенты Azure AD, которые принадлежат партнерам Майкрософт, которые являются либо частью поставщика облачных решений [Microsoft,](https://partnercenter.microsoft.com/en-us/partner/programs)Office 365 Syndication, либо партнерской программы Microsoft Advisor.

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Получение контрактов](../api/contract-get.md) | Контракт |Чтение свойств определенного объекта контракта. |
|[Список контрактов](../api/contract-list.md) | Коллекция контрактов | Список контрактов в клиенте-партнере. |

## <a name="properties"></a>Свойства
| Свойство   | Тип | Описание |
|:---------------|:--------|:----------|
|contractType|String|Тип контракта. Возможные значения:  `SyndicationPartner` , `BreadthPartner` , `ResellerPartner` . Подробнее в таблице [ниже](#contracttype-values).|
|customerId|Guid|Уникальный идентификатор клиента клиента, на который ссылается это партнерство. Соответствует свойству id ресурса организации клиента клиента. |
|defaultDomainName|String|Копия доменного имени клиента по умолчанию. Копия будет выполнена после того, как будет установлено партнерство с клиентом. Он не обновляется автоматически, если меняется имя домена клиента по умолчанию.|
|displayName|String|Копия отображаемого имени клиента. Копия будет выполнена после того, как будет установлено партнерство с клиентом. Оно не обновляется автоматически, если меняется имя отображения клиента.|
|id|String| Уникальный идентификатор для партнерства. Клавиша, только для чтения |

### <a name="contracttype-values"></a>значения contractType

|Member|Описание|
|:---|:---|
|SyndicationPartner|Партнер, *который исключительно перепродает* и управляет O365 и Intune для этого клиента. Они перепродают и поддерживают своих клиентов.|
|BreadthPartner|Партнер может оказывать административную поддержку этому клиенту. Однако партнер не имеет права перепродавать клиенту.|
|ResellerPartner|Партнер, аналогичный партнеру синдикации, за исключением того, что у партнера нет эксклюзивного доступа к клиенту. В случае синдикации клиент не может покупать дополнительные прямые подписки у Microsoft или у других партнеров.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.contract"
}-->

```json
{
  "contractType": "String",
  "customerId": "Guid",
  "defaultDomainName": "String",
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

