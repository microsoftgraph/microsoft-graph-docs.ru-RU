---
title: Обновление параметров
description: 'Обновление свойств объекта settings. '
author: jpettere
ms.localizationpriority: medium
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 8c78950129ccb0c469b505970c696a4b57236e9d
ms.sourcegitcommit: 94741ff7f61f20a39dacfa6ce451a77ca02dd68a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/14/2022
ms.locfileid: "62047107"
---
# <a name="update-settings"></a>Обновление параметров

Пространство имен: microsoft.graph

Обновление свойств объекта [userSettings.](../resources/usersettings.md) Пользователи в одной организации могут иметь различные параметры в зависимости от их предпочтений или политик организации. Чтобы получить текущие параметры пользователя, см. [текущие параметры пользователя.](usersettings-get.md) 

### <a name="batch-request"></a>Пакетный запрос

Кроме того, можно отключать несколько пользователей от Delve и отключить их вклад в доступ к контенту для всей организации с помощью пакетного запроса.
Дополнительные дополнительные информации см. в серии [JSON.](/graph/json-batching)

>**Важно.** Только члены группы [ролей](/exchange/permissions/permissions?view=exchserver-2019#role-groups) управления организацией могут обновлять несколько пользователей. 



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

## <a name="request-body"></a>Тело запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|Логический|Установите для true отключение доступа делегатов к API [Trending](/graph/api/resources/insights-trending?view=graph-rest-1.0) и отключение доступа к документам в Office Delve для пользователя. Значение true также влияет на релевантность контента, отображаемого в Microsoft 365 , например, рекомендуемые сайты в SharePoint Home и представление Discover в OneDrive для бизнеса показывают менее релевантные результаты. Этот параметр отражает состояние управления в [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).|

## <a name="example"></a>Пример 

##### <a name="request"></a>Запрос

Вот пример запроса о том, как отключать пользователя от Delve и отключить его вклад в содержимого для всей организации.

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
