---
title: Тип ресурса contract
description: Представляет существующее партнерство между клиентом партнера и клиентом пользователя.
localization_priority: Normal
ms.openlocfilehash: c14f4a51cbab5625c16ef0f0e515fffd35619366
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812301"
---
# <a name="contract-resource-type"></a>Тип ресурса contract
Представляет существующее партнерство между клиентом партнера и клиентом пользователя.

> **Важно!** Существует только в клиентах партнеров. Клиенты партнеров — это клиенты Azure AD, которые принадлежат партнерам корпорации Майкрософт, являющимся [поставщиками облачных решений (Майкрософт)](https://partnercenter.microsoft.com/en-us/partner/programs), участниками программы синдикации Office 365 или участниками партнерской программы Microsoft Advisor.

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Получение contract](../api/contract-get.md) | contract |Чтение свойств определенных объектов contract. |
|[Перечисление объектов contract](../api/contract-list.md) | Коллекция contract | Перечисление объектов contract в клиенте партнера. |

## <a name="properties"></a>Свойства
| Свойство   | Тип | Описание |
|:---------------|:--------|:----------|
|contractType|String|Тип контракта.<br><br>Возможные значения:<br> *SyndicationPartner*. Партнер, имеющий исключительные права на перепродажу Office 365 и Intune для этого пользователя, а также управление ими. Такие партнеры выполняют перепродажу и предоставляют пользователям поддержку.<br> *BreadthPartner*. Партнер может предоставлять пользователю административную поддержку. Прав на перепродажу этот партнер не имеет.<br>*ResellerPartner*. Этот тип партнеров аналогичен SyndicationPartner, но не предусматривает эксклюзивного доступа к клиенту. В случае SyndicationPartner пользователь не может приобретать дополнительные подписки непосредственно у корпорации Майкрософт или у других партнеров.|
|customerId|Guid|Уникальный идентификатор для клиента пользователя, указываемый в случае партнерства. Соответствует свойству id для ресурса организации клиента пользователя. |
|defaultDomainName|String|Копия стандартного доменного имени для клиента пользователя. Копия создается при установлении партнерства с пользователем. Она не обновляется автоматически, если изменяется стандартное доменное имя для клиента пользователя.|
|displayName|Строка|Копия отображаемого имени клиента пользователя. Копия создается при установлении партнерства с пользователем. Она не обновляется автоматически, если изменяется отображаемое имя клиента пользователя.|
|id|String| Уникальный идентификатор, заданный для партнерства. Ключ, только для чтения. |

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
