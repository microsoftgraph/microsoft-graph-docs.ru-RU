---
title: Тип ресурса externalIdentitiesPolicy
description: Представляет политику на уровне клиента, которая определяет, могут ли внешние пользователи покинуть клиент Azure AD с помощью элементов управления самообслуживания.
author: KuiGithui
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 49701027e0dace54a8f74a2eebef0115329de9a4
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768365"
---
# <a name="externalidentitiespolicy-resource-type"></a>Тип ресурса externalIdentitiesPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику на уровне клиента, которая определяет, могут ли внешние пользователи покинуть гостевой Azure AD с помощью элементов управления самообслуживания. Если это разрешено администратором, внешние пользователи могут выйти из гостевого Azure AD через меню  организаций на портале "Моя [учетная запись](https://myaccount.microsoft.com/)".

Наследуется [от policyBase](../resources/policybase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение externalIdentitiesPolicy](../api/externalidentitiespolicy-get.md)|[externalIdentitiesPolicy](../resources/externalidentitiespolicy.md)|Чтение свойств и связей объекта [externalIdentitiesPolicy](../resources/externalidentitiespolicy.md) .|
|[Обновление externalIdentitiesPolicy](../api/externalidentitiespolicy-update.md)|[externalIdentitiesPolicy](../resources/externalidentitiespolicy.md)|Обновление свойств объекта [externalIdentitiesPolicy](../resources/externalidentitiespolicy.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowDeletedIdentitiesDataRemoval|Логическое|Уведомляет Azure AD о том, следует ли удалять сведения о внешнем удостоверении из гостевого клиента при удалении пользователя в домашнем клиенте. |
|allowExternalIdentitiesToLeave|Логическое|Определяет, могут ли внешние пользователи покинуть гостевой клиент. Если задано значение , `false`элементы управления самообслуживания не включены, и администратор гостевого клиента должен вручную удалить внешнего пользователя из гостевого клиента.|
|displayName|String|Имя политики. Наследуется [от policyBase](../resources/policybase.md).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalIdentitiesPolicy",
  "baseType": "microsoft.graph.policyBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.externalIdentitiesPolicy",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "allowExternalIdentitiesToLeave": "Boolean",
  "allowDeletedIdentitiesDataRemoval": "Boolean"
}
```

