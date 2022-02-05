---
title: тип ресурса x509CertificateAuthenticationMethodConfiguration
description: 'Представляет сведения о родной службе проверки подлинности Azure AD Certificate-Based (CBA) в клиенте, в том числе о том, включен или отключен метод проверки подлинности, а также пользователи и группы, которые могут зарегистрировать и использовать его.'
author: charlenezheng
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="x509certificateauthenticationmethodconfiguration-resource-type"></a>тип ресурса x509CertificateAuthenticationMethodConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о родной службе проверки подлинности Azure AD Certificate-Based (CBA) в клиенте, в том числе о том, включен или отключен метод проверки подлинности, а также пользователи и группы, которые могут зарегистрировать и использовать его.

Наследуется от [проверки подлинностиMethodConfiguration](../resources/authenticationmethodconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get x509CertificateAuthenticationMethodConfiguration](../api/x509certificateauthenticationmethodconfiguration-get.md)|[x509CertificateAuthenticationMethodConfiguration](../resources/x509certificateauthenticationmethodconfiguration.md)|Ознакомьтесь с свойствами и отношениями объекта x509CertificateAuthenticationMethodConfiguration.|
|[Обновление x509CertificateAuthenticationMethodConfiguration](../api/x509certificateauthenticationmethodconfiguration-update.md)|[x509CertificateAuthenticationMethodConfiguration](../resources/x509certificateauthenticationmethodconfiguration.md)|Обновление свойств объекта x509CertificateAuthenticationMethodConfiguration.|
|[Удаление x509CertificateAuthenticationMethodConfiguration](../api/x509certificateauthenticationmethodconfiguration-delete.md)|Нет| Восстановление объекта x509CertificateAuthenticationMethodConfiguration в конфигурации по умолчанию.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор политики метода проверки подлинности. Значение всегда `X509Certificate`. Наследуется [от проверки подлинностиMethodConfiguration](../resources/authenticationmethodconfiguration.md).|
|state|authenticationMethodState|Возможные значения: `enabled`, `disabled`. Наследуется [от проверки подлинностиMethodConfiguration](../resources/authenticationmethodconfiguration.md).|
|certificateUserBindings|[коллекция x509CertificateUserBinding](../resources/x509certificateuserbinding.md)|Определяет поля в сертификате X.509, которые соединит атрибуты объекта пользователя Azure AD для привязки сертификата к пользователю. Приоритет **объекта** определяет порядок выполнения привязки. Первая привязка, которая будет использоваться для совпадений, а остальные игнорируются. |
|authenticationModeConfiguration|[x509CertificateAuthenticationModeConfiguration](../resources/x509certificateauthenticationmodeconfiguration.md)|Определяет сильные конфигурации проверки подлинности. Эта конфигурация включает режим проверки подлинности по умолчанию и различные правила для сильных привязки проверки подлинности. |


## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|includeTargets|[коллекция authenticationMethodTarget](../resources/authenticationmethodtarget.md)|Коллекция пользователей или групп, которые могут использовать метод проверки подлинности.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.x509CertificateAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.x509CertificateAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "certificateUserBindings": [
    {
      "@odata.type": "microsoft.graph.x509CertificateUserBinding"
    }
  ],
  "authenticationModeConfiguration": {
    "@odata.type": "microsoft.graph.x509CertificateAuthenticationModeConfiguration"
  }
}
```

