---
title: тип ресурса federatedIdentityCredential
description: Ссылки на федераированные учетные данные удостоверений приложения. Эти федераированные учетные данные удостоверений используются в федерации удостоверений рабочей нагрузки при обмене маркера от надежного эмитента на маркер доступа, связанный с приложением, зарегистрированным в Azure AD.
author: kjyam98
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: fb5d51cd16103c21656927b999bf5484d70d0800
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697451"
---
# <a name="federatedidentitycredential-resource-type"></a>тип ресурса federatedIdentityCredential

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ссылки на федераированные учетные данные удостоверений приложения. Эти федераированные учетные [](/azure/active-directory/develop/workload-identity-federation) данные удостоверений используются в федерации удостоверений рабочей нагрузки при обмене маркера от надежного эмитента на маркер доступа, связанный с приложением, зарегистрированным в Azure AD.

Наследует от [объекта](../resources/entity.md).

>**ПРИМЕЧАНИЕ:** Этот ресурс не доступен в [национальных облачных](/graph/deployments) развертываниях.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список federatedIdentityCredentials](../api/application-list-federatedidentitycredentials.md)|[federatedIdentityCredential](../resources/federatedidentitycredential.md) collection|Получите список объектов [federatedIdentityCredential](../resources/federatedidentitycredential.md) и их свойств.|
|[Создание federatedIdentityCredential](../api/application-post-federatedidentitycredentials.md)|[federatedIdentityCredential](../resources/federatedidentitycredential.md)|Создайте новый [объект federatedIdentityCredential.](../resources/federatedidentitycredential.md)|
|[Get federatedIdentityCredential](../api/federatedidentitycredential-get.md)|[federatedIdentityCredential](../resources/federatedidentitycredential.md)|Ознакомьтесь с свойствами и отношениями объекта [federatedIdentityCredential.](../resources/federatedidentitycredential.md)|
|[Обновление federatedIdentityCredential](../api/federatedidentitycredential-update.md)|Нет|Обновление свойств объекта [federatedIdentityCredential.](../resources/federatedidentitycredential.md)|
|[Удаление federatedIdentityCredential](../api/federatedidentitycredential-delete.md)|Нет|Удаляет объект [federatedIdentityCredential.](../resources/federatedidentitycredential.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| аудитории | Коллекция строк | Списки аудиторий, которые могут отображаться во внешнем маркере. Это поле является обязательным и по умолчанию "api://AzureADTokenExchange". В нем платформа удостоверений Майкрософт, что следует принять в `aud` утверждении в входящих маркерах. Это значение представляет Azure AD во внешнем поставщике удостоверений и не имеет фиксированного значения для поставщиков удостоверений , возможно, потребуется создать новую регистрацию приложений в поставщике удостоверений, чтобы служить аудиторией этого маркера. Обязательный. |
| description | String | Un-validated, user-provided description of the federated identity credential. Необязательный параметр.  |
| id| String | Уникальный идентификатор федераированной идентификации. Обязательно. Только для чтения.  |
| эмитент | String | URL-адрес внешнего поставщика удостоверений и должен соответствовать утверждению об обмене `issuer` внешнего маркера. Сочетание значений эмитента **и** субъекта должно **быть** уникальным в приложении. Обязательно. |
| name | String | является уникальным идентификатором для федератированных учетных данных удостоверений, который имеет ограничение символов в 120 символов и должен быть удобным URL-адресом. После создания она неуменяема. Обязательно. Значение null не допускается. Поддерживает `$filter` (`eq`). |
| subject | String | Обязательный. Идентификатор рабочей нагрузки внешнего программного обеспечения во внешнем поставщике удостоверений. Как и значение аудитории, он не имеет фиксированного формата, так как каждый поставщик удостоверений использует свои собственные — иногда GUID, иногда идентификатор двоеточия, иногда произвольные строки. Здесь значение должно соответствовать `sub` утверждению в маркере, представленном Azure AD. Сочетание **эмитента и** **субъекта должно** быть уникальным в приложении. Поддерживает `$filter` (`eq`). |


## <a name="relationships"></a>Связи

Нет


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.federatedIdentityCredential",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.federatedIdentityCredential",
  "name": "String",
  "issuer": "String",
  "subject": "String",
  "description": "String",
  "audiences": [
    "String"
  ]
}
```

