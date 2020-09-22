---
title: Тип ресурса Хомереалмдисковериполици
description: Представляет политику для управления поведением проверки подлинности Azure Active Directory для федеративных пользователей.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ab4cde183f07235f42886bf1dcaba53def9aa0ec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013603"
---
# <a name="homerealmdiscoverypolicy-resource-type"></a>Тип ресурса Хомереалмдисковериполици

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику для управления поведением проверки подлинности Azure Active Directory для федеративных пользователей, в частности для ограничений автоматического ускорения и проверки подлинности пользователей в федеративных доменах. Вы можете настроить Хомереалмдисковериполици для всех субъектов службы в организации или для определенных субъектов службы в Организации.  Дополнительные сведения о сценариях и политиках приведены [в статье Настройка режима входа в Azure AD для приложения с помощью политики обнаружения домашней области](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal).

Наследуется от [стсполици](stsPolicy.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание Хомереалмдисковериполици](../api/homerealmdiscoverypolicy-post-homerealmdiscoverypolicies.md) | [хомереалмдисковериполици](homerealmdiscoverypolicy.md) | Создание объекта Хомереалмдисковериполици. |
| [Получение Хомереалмдисковериполици](../api/homerealmdiscoverypolicy-get.md) | [хомереалмдисковериполици](homerealmdiscoverypolicy.md) | Чтение свойств и связей объекта Хомереалмдисковериполици. |
| [Перечисление типов ресурсов homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-list.md) | [хомереалмдисковериполици](homerealmdiscoverypolicy.md) | Чтение свойств и связей объектов ХомереалмдисковериполиЦиес. |
| [Обновление Хомереалмдисковериполици](../api/homerealmdiscoverypolicy-update.md) | Нет | Обновление объекта Хомереалмдисковериполици. |
| [Удаление Хомереалмдисковериполици](../api/homerealmdiscoverypolicy-delete.md) | Нет | Удаление объекта Хомереалмдисковериполици. |
| [Список appliesTo](../api/homerealmdiscoverypolicy-list-appliesto.md) | Коллекция [directoryObject](directoryobject.md) | Получение списка Директорйобжектс, к которым применена эта политика. |
| [Назначение типа ресурса homeRealmDiscoveryPolicy](../api/serviceprincipal-post-homerealmdiscoverypolicies.md) | Нет | Назначьте объект Хомереалмдисковериполици объекту [servicePrincipal](serviceprincipal.md) . |
| [Список назначенных Хомереалмдисковериполици](../api/serviceprincipal-list-homerealmdiscoverypolicies.md) | Коллекция [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) | Перечисление объектов Хомереалмдисковериполици, назначенных объекту [servicePrincipal](serviceprincipal.md) . |
| [Удаление типа ресурса homeRealmDiscoveryPolicy](../api/serviceprincipal-delete-homerealmdiscoverypolicies.md) | Нет | Удаление объекта Хомереалмдисковериполици из объекта [servicePrincipal](serviceprincipal.md) . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор для этой политики. Только для чтения.|
|RDLC|Коллекция String| Коллекция String, содержащая строку JSON, определяющую правила и параметры для этой политики. Ниже приведены дополнительные сведения о схеме JSON для этого свойства. Обязательный.|
|description|String| Описание для этой политики.|
|displayName|String| Отображаемое имя для этой политики. Обязательный.|
|исорганизатиондефаулт|Boolean|Если задано значение true, активируется эта политика. Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию. Необязательное значение по умолчанию — false.|


### <a name="properties-of-a-home-realm-discovery-policy-definition"></a>Свойства определения политики обнаружения домашней области
Свойства, приведенные ниже, формируют объект JSON, представляющий политику времени существования маркеров. Этот объект JSON необходимо **преобразовать в строку с escape-символами** , которые будут вставлены в свойство **definition** . Ниже показан пример в формате JSON.

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"HomeRealmDiscoveryPolicy\":
     {\"AccelerateToFederatedDomain\":true,
      \"PreferredDomain\":\"federated.example.edu\"}}"
  ]
```

| Свойство     | Тип   |Описание| 
|:---------------|:--------|:----------|
|акцелератетофедератеддомаин|Boolean| Задано значение `true` для автоускорения (обход поиска домашних областей). Если `true` в клиенте есть только один проверенный и федеративный домен, то пользователи будут передаваться непосредственно поставщику федеративного удостоверения (например, ADFS) для входа. Если `true` в клиенте имеется несколько проверенных доменов, необходимо указать **преферреддомаин** . Необязательно.|
|преферреддомаин|String| Указывает домен для ускорения входа в систему. Его можно опустить, если у клиента только один федеративный домен. Если он не указан и существует несколько проверенных федеративных доменов, эта политика не оказывает никакого действия. Обязательный, если **акцелератетофедератеддомаин** — `true` .|
|алловклаудпассвордвалидатион|Boolean| Чтобы `true` разрешить приложению выполнять проверку подлинности федеративного пользователя, указав учетные данные имени пользователя и пароля непосредственно в конечной точке маркера Azure Active Directory. Работает, только если включена синхронизация хэша паролей. Необязательно.|

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
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
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
  "description": "homeRealmDiscoveryPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

