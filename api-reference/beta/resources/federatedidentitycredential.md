---
title: Тип ресурса federatedIdentityCredential
description: Ссылается на учетные данные федеративного удостоверения приложения. Эти учетные данные федеративного удостоверения используются в федерации удостоверений рабочей нагрузки при обмене маркера от доверенного издателя на маркер доступа, связанный с приложением, зарегистрированным в Azure AD.
author: shahzad-khalid
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 4a529d1079c3058a1cb381e8b46c7849d8d4f3dd
ms.sourcegitcommit: 995056279c2151d7ce4a0fcff067fbc6edced728
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2022
ms.locfileid: "65602744"
---
# <a name="federatedidentitycredential-resource-type"></a>Тип ресурса federatedIdentityCredential

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ссылается на учетные данные федеративного удостоверения приложения. Эти учетные данные федеративного удостоверения используются в федерации удостоверений рабочей нагрузки при обмене маркера от доверенного издателя на маркер доступа, связанный с приложением, зарегистрированным Azure AD.[](/azure/active-directory/develop/workload-identity-federation)

Наследует [от сущности](../resources/entity.md).

>**ПРИМЕЧАНИЕ:** Этот ресурс недоступен в [национальных облачных](/graph/deployments) развертываниях.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление federatedIdentityCredentials](../api/application-list-federatedidentitycredentials.md)|Коллекция [federatedIdentityCredential](../resources/federatedidentitycredential.md)|Получение списка объектов [federatedIdentityCredential](../resources/federatedidentitycredential.md) и их свойств.|
|[Создание federatedIdentityCredential](../api/application-post-federatedidentitycredentials.md)|[federatedIdentityCredential](../resources/federatedidentitycredential.md)|Создайте объект [federatedIdentityCredential](../resources/federatedidentitycredential.md) .|
|[Получение federatedIdentityCredential](../api/federatedidentitycredential-get.md)|[federatedIdentityCredential](../resources/federatedidentitycredential.md)|Чтение свойств и связей объекта [federatedIdentityCredential](../resources/federatedidentitycredential.md) .|
|[Обновление federatedIdentityCredential](../api/federatedidentitycredential-update.md)|Нет|Обновление свойств объекта [federatedIdentityCredential](../resources/federatedidentitycredential.md) .|
|[Удаление federatedIdentityCredential](../api/federatedidentitycredential-delete.md)|Нет|Удаляет объект [federatedIdentityCredential](../resources/federatedidentitycredential.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| Аудитории | Коллекция String | Список аудиторий, которые могут отображаться во внешнем маркере. Это поле является обязательным и по умолчанию имеет значение "api://AzureADTokenExchange". В нем указано, платформа удостоверений Майкрософт должны приниматься в утверждении `aud` во входящем токене. Это значение Azure AD во внешнем поставщике удостоверений и не имеет фиксированного значения для поставщиков удостоверений. Возможно, потребуется создать регистрацию приложения в поставщике удостоверений, чтобы выступать в качестве аудитории этого маркера. Обязательный. |
| description | Строка | Не проверенное пользователем описание учетных данных федеративного удостоверения. Необязательно.  |
| id| String | Уникальный идентификатор федеративного удостоверения. Обязательный аргумент. Только для чтения.  |
| Эмитента | Строка | URL-адрес внешнего поставщика удостоверений и должен соответствовать утверждению `issuer` внешнего маркера, для которого выполняется обмен. Сочетание значений издателя и субъекта **должно быть уникальным** в приложении. Обязательный аргумент. |
| name | String | — это уникальный идентификатор для учетных данных федеративного удостоверения, который имеет ограничение в 120 символов и должен быть понятным по URL-адресу. После создания она неизменяема. Обязательно. Значение null не допускается. Поддерживает `$filter` (`eq`). |
| subject | String | Обязательный. Идентификатор рабочей нагрузки внешнего программного обеспечения во внешнем поставщике удостоверений. Как и значение аудитории, он не имеет фиксированного формата, так как каждый поставщик удостоверений использует собственный идентификатор GUID, иногда идентификатор с разделителями двоеточия, иногда произвольные строки. Здесь значение должно соответствовать утверждению `sub` в токене, представленном Azure AD. Сочетание **издателя и субъекта** **должно** быть уникальным в приложении. Поддерживает `$filter` (`eq`). |


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

