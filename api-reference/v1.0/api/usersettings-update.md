---
title: Обновление параметров
description: 'Обновление свойств объекта settings. '
author: jpettere
ms.localizationpriority: medium
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 5812fb25f03a1bffde622ac1461738754b060b65
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768121"
---
# <a name="update-settings"></a>Обновление параметров

Пространство имен: microsoft.graph

Обновление свойств объекта [userSettings](../resources/usersettings.md) . Пользователи в одной организации могут иметь разные параметры в зависимости от их предпочтений или политик организации. Чтобы получить текущие параметры пользователя, ознакомьтесь [с текущими параметрами пользователя](usersettings-get.md). 

### <a name="batch-request"></a>Пакетный запрос

Кроме того, можно отказаться от использования Delve несколькими пользователями и отключить их вклад в релевантность содержимого для всей организации с помощью пакетного запроса.
Дополнительные сведения см. в статье [о пакетной обработке JSON](/graph/json-batching).

>**Важно**! Обновить несколько пользователей могут [только члены](/exchange/permissions/permissions?view=exchserver-2019#role-groups&preserve-view=true) группы ролей управления организации. 



## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.ReadWrite, User.ReadWrite.All   |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | User.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

```http
PATCH /me/settings
```

Запрос с параметрами user id или userPrincipalName доступен только пользователю или пользователю с разрешениями User.ReadWrite.All. Дополнительные сведения см. в статье [Разрешения](/graph/permissions-reference). 

```http
PATCH /users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение|
|:-----------|:------|
| Авторизация  | Bearer {token}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|Логический|Задайте значение true: отключите делегированный доступ к API ["](/graph/api/resources/insights-trending?view=graph-rest-1.0&preserve-view=true) Тенденции" и отключите доступ к документам в Office Delve для пользователя. Значение true также влияет на релевантность содержимого, отображаемого в Microsoft 365. Например, рекомендуемые сайты в Домашней папке SharePoint и представление обнаружения в OneDrive для бизнеса отображают менее релевантные результаты. Этот параметр отражает состояние элемента управления [в Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).|

## <a name="example"></a>Пример 

##### <a name="request"></a>Запрос

Ниже приведен пример запроса на отказ пользователя от Delve и отключение его вклада в релевантность содержимого для всей организации.

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
Content-type: application/json

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a>Отклик

Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```
