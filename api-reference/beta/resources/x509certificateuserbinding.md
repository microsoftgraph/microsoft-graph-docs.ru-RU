---
title: тип ресурса x509CertificateUserBinding
description: 'Определяет поля в сертификате X.509, которые соотносят с атрибутами объекта пользователя Azure AD, чтобы привязать сертификат к учетной записи пользователя.'
author: charlenezheng
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="x509certificateuserbinding-resource-type"></a>тип ресурса x509CertificateUserBinding

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет поля в сертификате X.509, которые соотносят с атрибутами объекта пользователя Azure AD, чтобы привязать сертификат к учетной записи пользователя.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|priority|Int32|Приоритет привязки. Azure AD использует привязку с наивысшим приоритетом. Это значение должно быть неоспоримым и уникальным в коллекции объектов в свойстве **certificateUserBindings** объекта **x509CertificateAuthenticationMethodConfiguration** . Обязательный|
|userProperty|Строка|Определяет свойство пользователя Azure AD объекта пользователя, используемого для привязки. Возможные значения: **userPrincipalName**, `onPremisesUserPrincipalName`, `email`. Обязательный.|
|x509CertificateField|String|Поле в сертификате X.509, используемом для привязки. Возможные значения: `PrincipalName`, `RFC822Name`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.x509CertificateUserBinding"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.x509CertificateUserBinding",
  "x509CertificateField": "String",
  "userProperty": "String",
  "priority": "Integer"
}
```

