---
title: тип ресурса featureRolloutPolicy
description: Представляет политику выкатки функций, связанную с объектом каталога.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 7fa35d99c8c77240a182b5d28a0fdb896153aa8b
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961137"
---
# <a name="featurerolloutpolicy-resource-type"></a>тип ресурса featureRolloutPolicy

Пространство имен: microsoft.graph

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику выкатки функций, связанную с объектом каталога. Создание политики внедрения компонентов помогает администраторам клиентов пилотным функциям Azure AD с определенной группой, прежде чем включать функции для всей организации. Это минимизирует влияние и помогает администраторам постепенно тестировать и выкатывать связанные функции проверки подлинности.

Ниже представлены ограничения для выкатки функций:

- Каждая функция поддерживает не более 10 групп.
- Поле **appliesTo** поддерживает только группы.
- Динамические группы и вложенные группы не поддерживаются.

Ниже представлены предварительные требования к каждому из компонентов, которые в настоящее время поддерживаются для выкатки с помощью этой политики.

### <a name="passthrough-authentication"></a>Проверка подлинности через проход

* Определите сервер с Windows Server 2012 R2 или более поздней версии, на котором необходимо запустить агент [PassthroughAuthentication.](/azure/active-directory/hybrid/how-to-connect-pta)Убедитесь, что сервер соединен с доменом, может проверить подлинность выбранных пользователей с помощью Active Directory и взаимодействовать с Azure AD в исходящие порты и URL-адреса.
* [Скачайте](https://aka.ms/getauthagent) & установите агент проверки подлинности Microsoft Azure AD Connect на сервере.
* Чтобы обеспечить высокую доступность, установите дополнительные агенты проверки подлинности на других серверах, как описано [здесь.](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability)
* Убедитесь, что вы правильно настроили параметры [smart lockout.](/azure/active-directory/authentication/howto-password-smart-lockout) Это необходимо для обеспечения того, чтобы учетные записи активных каталогов пользователей не блокировалися плохими субъектами.

### <a name="seamlesssso"></a>SeamlessSso

* Включить [SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) для лесов AD на основе [этих](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) инструкций.

### <a name="passwordhashsync"></a>PasswordHashSync

* Включении [PasswordHashSync со](/azure/active-directory/hybrid/whatis-phs)   страницы "Необязательные функции" в Azure AD Connect.

### <a name="emailasalternateid"></a>EmailAsAlternateId

* Связывать альтернативные сообщения электронной почты с учетными записями пользователей.

## <a name="methods"></a>Методы

| Метод                                                                         | Возвращаемый тип                                     | Описание                                                               |
|:-------------------------------------------------------------------------------|:------------------------------------------------|:--------------------------------------------------------------------------|
| [Функция ListRolloutPolicies](../api/list-featurerolloutpolicies.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Извлечение списка объектов featureRolloutPolicy.                          |
| [Get featureRolloutPolicy](../api/featurerolloutpolicy-get.md)                 | [featureRolloutPolicy](featurerolloutpolicy.md) | Извлечение свойств и связей объекта featurerolloutpolicy. |
| [Создание featureRolloutPolicy](../api/post-featurerolloutpolicies.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Создайте новый объект featureRolloutPolicy.                                 |
| [Обновление функцииRolloutPolicy](../api/featurerolloutpolicy-update.md)           | [featureRolloutPolicy](featurerolloutpolicy.md) | Обновление свойств объекта featurerolloutpolicy.                     |
| [Удаление featureRolloutPolicy](../api/featurerolloutpolicy-delete.md)           | Нет                                            | Удаление объекта featureRolloutPolicy.                                     |
| [Назначение appliesTo](../api/featurerolloutpolicy-post-appliesto.md)              | [directoryObject](directoryobject.md)           | Назначение каталогаОбект для выкатки функций.                              |
| [Удаление appliesTo](../api/featurerolloutpolicy-delete-appliesto.md)            | Нет                                            | Удалите directoryObject из выкатки функций.                            |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|String|Описание этой политики выкатки функций.|
|displayName|String|Имя отображения для этой политики выкатки функций.|
|функция|stagedFeatureName| Возможные значения: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `emailAsAlternateId`, `unknownFutureValue`.|
|id|String| Только для чтения.|
|isAppliedToOrganization|Логический|Указывает, следует ли применять эту политику выкатки функций ко всей организации.|
|isEnabled|Boolean|Указывает, включена ли выкатка функций.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|appliesTo|Коллекция [directoryObject](directoryobject.md)| Допускается значение null. Указывает список directoryObjects, для которые включена функция.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "feature": "string",
  "id": "String (identifier)",
  "isAppliedToOrganization": false,
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "featureRolloutPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


