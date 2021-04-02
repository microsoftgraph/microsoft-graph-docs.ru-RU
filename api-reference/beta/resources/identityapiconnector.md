---
title: тип ресурса identityApiConnector
description: Представляет соединители API в клиенте Azure Active Directory.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f7ecb96a9ca2f4397c1f0ee52908a7802374df0f
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508108"
---
# <a name="identityapiconnector-resource-type"></a>тип ресурса identityApiConnector

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет соединители API в клиентах Azure Active Directory (Azure AD) и Azure AD B2C.

Соединитель API, используемый в вашей самообслуживке Azure AD External Identities и потоках пользователей для регистрации Azure AD B2C, позволяет вызывать API во время выполнения потока пользователей. Соединителя API предоставляет сведения, необходимые для вызова API, включая URL-адрес конечной точки и проверку подлинности. Соединители API можно использовать на определенном шаге в потоке пользователей, чтобы повлиять на выполнение потока пользователей. Например, ответ API может заблокировать регистрацию пользователя, показать ошибку проверки ввода или переписать собранные атрибуты пользователя.

Используйте [API b2xIdentityUserFlow](b2xidentityuserflow.md) для использования соединителю API из потока пользователей самообслуживания внешних удостоверений.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список](../api/identityapiconnector-list.md)|[коллекция identityApiConnector](identityapiconnector.md)| Получить список соединителов API|
|[Создание](../api/identityapiconnector-create.md)|[identityApiConnector](identityapiconnector.md)|Создание нового соединитетеля API. |
|[Получение](../api/identityapiconnector-get.md)|[identityApiConnector](identityapiconnector.md)|Ознакомьтесь с свойствами [объекта identityApiConnector.](../resources/identityapiconnector.md)|
|[Обновление](../api/identityapiconnector-update.md)|[identityApiConnector](identityapiconnector.md)|Обновление свойств соединиттеля API.|
|[Загрузка клиентского сертификата](../api/identityapiconnector-uploadclientcertificate.md)|[identityApiConnector](identityapiconnector.md)|Загрузите клиентский сертификат для проверки подлинности.|
|[Удаление](../api/identityapiconnector-delete.md)|Нет|Удаление соединитетеля API.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Случайно созданный ID соединиттеля API. |
|displayName|String| Имя соединитетеля API. |
|targetUrl|String| URL-адрес конечной точки API для вызова. |
|проверка подлинностиКонфигурация|[apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md)|Объект, описывая сведения о конфигурации проверки подлинности для вызова API. Поддерживается клиентский сертификат Basic и PKCS 12.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityApiConnector",
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
