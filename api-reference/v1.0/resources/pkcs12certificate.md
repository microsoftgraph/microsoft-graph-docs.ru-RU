---
title: тип ресурса pkcs12Certificate
description: Представляет конфигурацию для загрузки pkcs12Certificate.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 60350908901293ec9bf090c9e2bc174d70c922e5
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882443"
---
# <a name="pkcs12certificate-resource-type"></a>тип ресурса pkcs12Certificate

Пространство имен: microsoft.graph

Представляет конфигурацию, используемую для отправки сертификата при использовании проверки подлинности клиентского сертификата HTTPS для вызова конечной точки соединителя API. Проверка подлинности клиентского сертификата — это взаимная проверка подлинности на основе сертификата, в которой клиент предоставляет клиентский сертификат конечной точке API для проверки его подлинности. Настроенный сертификат соединиттеля API отправляется Azure AD в конечную точку API, которая затем проверяет сертификат.

Наследует [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|pkcs12Value|Строка| Представляет отправленное содержимое pfx. Значение должно быть кодированной версией базового-64 фактического контента сертификата. Обязательно.|
|password|Строка| Пароль для файла pfx. Обязательно. Если пароль не используется, необходимо предоставить значение `""` .|

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
