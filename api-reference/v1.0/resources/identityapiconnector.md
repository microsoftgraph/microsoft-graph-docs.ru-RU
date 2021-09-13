---
title: тип ресурса identityApiConnector
description: Представляет соединители API в Azure Active Directory клиента.
author: nickgmicrosoft
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 05c51b2468885daea730e597b2c4f7172699c28f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098967"
---
# <a name="identityapiconnector-resource-type"></a>тип ресурса identityApiConnector

Пространство имен: microsoft.graph

Представляет соединители API в Azure Active Directory клиентах Azure AD.

Соединитель API, используемый в потоках пользователей самообслуживаемой регистрации Azure AD External Identities, позволяет вызывать API во время выполнения потока пользователей. Соединителя API предоставляет сведения, необходимые для вызова API, включая URL-адрес конечной точки и проверку подлинности. Соединители API можно использовать на определенном шаге в потоке пользователей, чтобы повлиять на выполнение потока пользователей. Например, ответ API может заблокировать регистрацию пользователя, показать ошибку проверки ввода или переписать собранные атрибуты пользователя.

Используйте [API b2xIdentityUserFlow](b2xidentityuserflow.md) для использования соединителю API из потока пользователей самообслуживания внешних удостоверений.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление](../api/identityapiconnector-list.md)|коллекция [identityApiConnector](../resources/identityapiconnector.md)| Получить список соединителов API|
|[Создание](../api/identityapiconnector-create.md)|[identityApiConnector](identityapiconnector.md)|Создание нового соединитетеля API. |
|[получение](../api/identityapiconnector-get.md);|[identityApiConnector](identityapiconnector.md)|Ознакомьтесь с свойствами [объекта identityApiConnector.](../resources/identityapiconnector.md)|
|[Обновление](../api/identityapiconnector-update.md)|[identityApiConnector](identityapiconnector.md)|Обновление свойств соединиттеля API.|
|[Upload клиентского сертификата](../api/identityapiconnector-uploadclientcertificate.md)|[identityApiConnector](identityapiconnector.md)|Upload клиентский сертификат для проверки подлинности.|
|[удаление](../api/identityapiconnector-delete.md);|Нет|Удаление соединитетеля API.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Случайно созданный идентификатор соединиттеля API. |
|displayName|Строка| Имя соединитетеля API. |
|targetUrl|String| URL-адрес конечной точки API для вызова. |
|проверка подлинностиКонфигурация|[apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md)|Объект, описывая сведения о конфигурации проверки подлинности для вызова API. Поддерживается клиентский сертификат Basic и PKCS 12.|

## <a name="relationships"></a>Отношения

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
