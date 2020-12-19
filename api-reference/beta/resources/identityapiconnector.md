---
title: Тип ресурса identityApiConnector
description: Представляет соединители API в клиенте Azure Active Directory.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6098b146b5117332df36b76adcbce95698d6041d
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720460"
---
# <a name="identityapiconnector-resource-type"></a>Тип ресурса identityApiConnector

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет соединители API в клиентах Azure Active Directory (Azure AD) и Azure AD B2C.

Соединитель API, используемый при самостоятельной регистрации внешних удостоверений Azure AD и потоках регистрации пользователей Azure AD B2C, позволяет вызывать API во время выполнения пользовательского потока. Соединителение API предоставляет сведения, необходимые для вызова API, включая URL-адрес конечной точки и проверку подлинности. Соединители API можно использовать на определенном этапе пользовательского потока, чтобы повлиять на выполнение пользовательского потока. Например, ответ API может блокировать регистрацию пользователя, показывать ошибку проверки ввода или переописывать собранные пользователем атрибуты.

Используйте API [b2xIdentityUserFlow](b2xidentityuserflow.md) для использования соединителю API из пользовательского потока самостоятельной регистрации внешних удостоверений.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список](../api/identityapiconnector-list.md)|[Коллекция identityApiConnector](identityapiconnector.md)| Получить список соединителов API|
|[создание](../api/identityapiconnector-create.md);|[identityApiConnector](identityapiconnector.md)|Создайте соединители API. |
|[получение](../api/identityapiconnector-get.md);|[identityApiConnector](identityapiconnector.md)|Чтение свойств объекта [identityApiConnector.](../resources/identityapiconnector.md)|
|[обновление](../api/identityapiconnector-update.md).|[identityApiConnector](identityapiconnector.md)|Обновление свойств соединители API.|
|[удаление](../api/identityapiconnector-delete.md);|Нет|Удаление соединители API.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Случайным образом созданный ИД соединителю API. |
|displayName|String| Имя соединители API. |
|targetUrl|String| URL-адрес конечной точки API для вызова. |
|authenticationConfiguration|[apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md)|Объект, который описывает сведения о конфигурации проверки подлинности для вызова API. В [настоящее время поддерживается](basicauthentication.md) только базовая проверка подлинности.|

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityApiConnector",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityApiConnector",
  "id": "String (identifier)",
  "displayName": "String",
  "targetUrl": "String",
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.apiAuthenticationConfigurationBase"
  }
}
```
