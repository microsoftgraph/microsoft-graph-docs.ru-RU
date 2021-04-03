---
title: тип ресурса pkcs12Certificate
description: Представляет конфигурацию для загрузки pkcs12Certificate в вызове API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f312a7be0bd29d57c1a6b7dc5c7e5d72e6d41206
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509404"
---
# <a name="pkcs12certificate-resource-type"></a>тип ресурса pkcs12Certificate

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет конфигурацию, используемую **для** отправки сертификата при использовании проверки подлинности клиентского сертификата HTTPS для вызова конечной точки соединителя API. Проверка подлинности клиентского сертификата — это взаимная проверка подлинности на основе сертификата, в которой клиент предоставляет клиентский сертификат конечной точке API для проверки его подлинности. Настроенный сертификат соединиттеля API отправляется Azure AD в конечную точку API, которая затем проверяет сертификат.

Наследует [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|pkcs12Value|String| Это поле для отправки контента pfx. Значение должно быть кодированной версией базового-64 фактического контента сертификата. Обязательно.|
|password|Строка| Это пароль для файла pfx. Обязательно. Если пароль не используется, необходимо по-прежнему предоставлять значение `""` .|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.pkcs12Certificate"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.pkcs12Certificate",
  "pkcs12Value": "String",
  "password": "String"
}
```
