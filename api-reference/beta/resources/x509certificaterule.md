---
title: тип ресурса x509CertificateRule
description: Определяет строгие правила настройки проверки подлинности для сертификата X.509. Правила настроены в дополнение к режиму проверки подлинности.
author: charlenezheng
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="x509certificaterule-resource-type"></a>тип ресурса x509CertificateRule

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет строгие правила настройки проверки подлинности для сертификата X.509. Правила настроены в дополнение к режиму проверки подлинности.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|идентификатор|Строка| Идентификатор сертификата X.509. Обязательный.|
|x509CertificateAuthenticationMode|x509CertificateAuthenticationMode| Тип сильного режима проверки подлинности. Допустимые значения: `x509CertificateSingleFactor`, `x509CertificateMultiFactor`, `unknownFutureValue`. Обязательный.|
|x509CertificateRuleType|x509CertificateRuleType| Тип правила конфигурации режима сертификата X.509. Допустимые значения: `issuerSubject`, `policyOID`, `unknownFutureValue`. Обязательный.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.x509CertificateRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.x509CertificateRule",
  "x509CertificateRuleType": "String",
  "identifier": "String",
  "x509CertificateAuthenticationMode": "String"
}
```

