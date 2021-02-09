---
title: Тип ресурса featureRolloutPolicy
description: Представляет политику выката функций, связанную с объектом каталога.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fa572cf9140a00d28b9db9d0e6a8e58fe6bb8969
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161672"
---
# <a name="featurerolloutpolicy-resource-type"></a>Тип ресурса featureRolloutPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику выката функций, связанную с объектом каталога. Создание политики внедрения компонентов помогает администраторам клиентов пилотным функциям Azure AD с определенной группой перед включением функций для всей организации. Это минимизирует влияние и помогает администраторам постепенно тестировать и тестировать связанные функции проверки подлинности.

Ниже данная возможность может быть ограниченной.

- Каждая функция поддерживает не более 10 групп.
- Поле **appliesTo** поддерживает только группы.
- Динамические и вложенные группы не поддерживаются.

Ниже представлены предварительные требования для каждой функции, которая в настоящее время используется для применения этой политики.

### <a name="passthrough-authentication"></a>Passthrough Authentication

* Определите сервер под управлением Windows Server 2012 R2 или более поздней версии, на котором должен работать агент [PassthroughAuthentication.](/azure/active-directory/hybrid/how-to-connect-pta)Убедитесь, что сервер присоединяется к домену, может проверить подлинность выбранных пользователей с помощью Active Directory и взаимодействовать с Azure AD через исходящие порты и URL-адреса.
* [Загрузите](https://aka.ms/getauthagent) & установить агент проверки подлинности Microsoft Azure AD Connect на сервере.
* Чтобы обеспечить высокую доступность, установите дополнительные агенты проверки подлинности на другие серверы, как [описано здесь.](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability)
* Убедитесь, что вы правильно настроили параметры [интеллектуальной](/azure/active-directory/authentication/howto-password-smart-lockout) блокировки. Это необходимо для того, чтобы учетные записи пользователей в локальной службе Active Directory не блокировали плохо активные субъекты.

### <a name="seamlesssso"></a>SeamlessSso

* В этом режиме в лесах AD в соответствии с этими [инструкциями](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) включается [seamlessSso.](/azure/active-directory/hybrid/how-to-connect-sso)

### <a name="passwordhashsync"></a>PasswordHashSync

* Включении [PasswordHashSync](/azure/active-directory/hybrid/whatis-phs)со страницы "Необязательные   функции" в Azure AD Connect.

### <a name="emailasalternateid"></a>EmailAsAlternateId

* Связывать альтернативную электронную почту с учетными записями пользователей.

## <a name="methods"></a>Методы

| Метод                                                                         | Возвращаемый тип                                     | Описание                                                               |
|:-------------------------------------------------------------------------------|:------------------------------------------------|:--------------------------------------------------------------------------|
| [Список featureRolloutPolicies](../api/directory-list-featurerolloutpolicies.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Получить список объектов featureRolloutPolicy.                          |
| [Get featureRolloutPolicy](../api/featurerolloutpolicy-get.md)                 | [featureRolloutPolicy](featurerolloutpolicy.md) | Извлечение свойств и связей объекта featurerolloutpolicy. |
| [Создание featureRolloutPolicy](../api/directory-post-featurerolloutpolicies.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Создание объекта featureRolloutPolicy.                                 |
| [Обновление featureRolloutPolicy](../api/featurerolloutpolicy-update.md)           | [featureRolloutPolicy](featurerolloutpolicy.md) | Обновление свойств объекта featurerolloutpolicy.                     |
| [Удаление featureRolloutPolicy](../api/featurerolloutpolicy-delete.md)           | Нет                                            | Удаление объекта featureRolloutPolicy.                                     |
| [Assign appliesTo](../api/featurerolloutpolicy-post-appliesto.md)              | [directoryObject](directoryobject.md)           | Назначьте directoryObject для выдаваемой функции.                              |
| [Remove appliesTo](../api/featurerolloutpolicy-delete-appliesto.md)            | Нет                                            | Удаление directoryObject из проектов функций.                            |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|String|Описание этой политики выката функций.|
|displayName|String|Отображаемого имени для этой политики выката функций.|
|feature|stagedFeatureName| Возможные значения: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.|
|id|String| Только для чтения.|
|isAppliedToOrganization|Boolean|Указывает, следует ли применять эту политику для всей организации.|
|isEnabled|Boolean|Указывает, включен ли выкат функции.|

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


