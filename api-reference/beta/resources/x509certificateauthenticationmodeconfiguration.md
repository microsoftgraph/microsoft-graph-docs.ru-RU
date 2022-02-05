---
title: тип ресурса x509CertificateAuthenticationModeConfiguration
description: Определяет сильные конфигурации проверки подлинности для сертификата X.509. Эта конфигурация включает режим проверки подлинности по умолчанию и различные правила привязки к проверке подлинности.
author: charlenezheng
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="x509certificateauthenticationmodeconfiguration-resource-type"></a>тип ресурса x509CertificateAuthenticationModeConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет сильные конфигурации проверки подлинности для сертификата X.509. Эта конфигурация включает режим проверки подлинности по умолчанию и различные правила привязки к проверке подлинности.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|правила|[коллекция x509CertificateRule](../resources/x509certificaterule.md)| Правила настроены в дополнение к режиму проверки подлинности для привязки определенного **x509CertificateRuleType** к **x509CertificateAuthenticationMode**. Например, привязать идентификатор `policyOID` к `1.32.132.343` режиму `x509CertificateMultiFactor` проверки подлинности.|
|x509CertificateAuthenticationDefaultMode|x509CertificateAuthenticationMode| Тип сильного режима проверки подлинности. Допустимые значения: `x509CertificateSingleFactor`, `x509CertificateMultiFactor`, `unknownFutureValue`.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.x509CertificateAuthenticationModeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.x509CertificateAuthenticationModeConfiguration",
  "x509CertificateAuthenticationDefaultMode": "String",
  "rules": [
    {
      "@odata.type": "microsoft.graph.x509CertificateRule"
    }
  ]
}
```

