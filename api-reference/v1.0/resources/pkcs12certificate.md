---
title: тип ресурса pkcs12Certificate
description: Представляет конфигурацию для загрузки pkcs12Certificate.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 273a1810a11e87c1981f7db2570e1773349435e981f9199b22017a35ced5b6e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54159830"
---
# <a name="pkcs12certificate-resource-type"></a>тип ресурса pkcs12Certificate

Пространство имен: microsoft.graph

Представляет конфигурацию, используемую для отправки сертификата при использовании проверки подлинности клиентского сертификата HTTPS для вызова конечной точки соединителя API. Проверка подлинности клиентского сертификата — это взаимная проверка подлинности на основе сертификата, в которой клиент предоставляет клиентский сертификат конечной точке API для проверки его подлинности. Настроенный сертификат соединиттеля API отправляется Azure AD в конечную точку API, которая затем проверяет сертификат.

Наследует [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|pkcs12Value|String| Представляет отправленное содержимое pfx. Значение должно быть кодированной версией базового-64 фактического контента сертификата. Обязательный элемент.|
|password|Строка| Пароль для файла pfx. Обязательный элемент. Если пароль не используется, необходимо предоставить значение `""` .|

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
