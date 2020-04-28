---
title: Тип ресурса Токенлифетимеполици
description: Представляет политику, которая может управлять временем существования маркера доступа, выданного Azure Active Directory.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 149c131ee38dc802de8845729ae1266a74eb8e4d
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917364"
---
# <a name="tokenlifetimepolicy-resource-type"></a>Тип ресурса Токенлифетимеполици

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику, которая может управлять жизненным циклом маркера доступа JWT, маркером ID или маркером SAML 1.1/2.0, выданным Azure Active Directory (Azure AD). Вы можете задать время жизни маркеров для всех приложений в Организации, для приложения с несколькими клиентами (многоорганизации) или для определенного субъекта-службы в Организации.  Дополнительные сведения о сценариях см [в разделе Настраиваемые сроки жизни маркеров в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

>Note: Настройка этой политики для маркеров обновления и маркеров сеансов не поддерживается.

Наследуется от [стсполици](stsPolicy.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание Токенлифетимеполици](../api/tokenlifetimepolicy-post-tokenlifetimepolicies.md) | [токенлифетимеполици](tokenlifetimepolicy.md) | Создание объекта Токенлифетимеполици. |
| [Получение Токенлифетимеполици](../api/tokenlifetimepolicy-get.md) | [токенлифетимеполици](tokenlifetimepolicy.md) | Чтение свойств и связей объекта Токенлифетимеполици. |
| [Перечисление типов ресурсов tokenLifetimePolicy](../api/tokenlifetimepolicy-list.md) | [токенлифетимеполици](tokenlifetimepolicy.md) | Чтение свойств и связей объектов ТокенлифетимеполиЦиес. |
| [Обновление Токенлифетимеполици](../api/tokenlifetimepolicy-update.md) | Нет | Обновление объекта Токенлифетимеполици. |
| [Удаление Токенлифетимеполици](../api/tokenlifetimepolicy-delete.md) | Нет | Удаление объекта Токенлифетимеполици. |
| [Список appliesTo](../api/tokenlifetimepolicy-list-appliesto.md) | Коллекция [directoryObject](directoryobject.md) | Получение списка Директорйобжектс, к которым применена эта политика. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор для этой политики. Только для чтения.|
|RDLC|Коллекция объектов string| Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики. Ниже приведены дополнительные сведения о схеме JSON для этого свойства. Обязательный.|
|description|String| Описание для этой политики.|
|displayName|Строка| Отображаемое имя для этой политики. Обязательный.|
|исорганизатиондефаулт|Boolean|Если задано значение true, активируется эта политика. Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию. Необязательное значение по умолчанию — false.|


### <a name="properties-of-a-token-lifetime-policy-definition"></a>Свойства определения политики времени существования маркера
Свойства, приведенные ниже, формируют объект JSON, представляющий политику времени существования маркеров. Этот объект JSON необходимо **преобразовать в строку с escape-символами** , которые будут вставлены в свойство **definition** . Ниже показан пример в формате JSON.

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"
  ]
```

>Note: все временные интервалы в этих свойствах указаны в формате "DD. чч: мм: СС".

>Note: Max Values для свойств, обозначенных в "Days", — 1 секунды, обозначенное как количество дней. Например, максимальное значение в 1 день задается как "23:59:59".

| Свойство     | Тип   |Описание| Минимальное значение | Максимальное значение | Значение по умолчанию|
|:---------------|:--------|:----------|:--------|:--------|:----|
|акцесстокенлифетиме|String|Управляет тем, как долго считаются действительными маркеры доступа и ИДЕНТИФИКАТОРы.|10 минут|1 день|1 час|
|Версия|Целое число|Установите значение 1. Обязательный.|Нет|Нет|Нет|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|Тег|Коллекция [directoryObject](directoryobject.md)| Коллекция [directoryObject](directoryObject.md) , к которой применена эта политика. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": true,
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tokenLifetimePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->