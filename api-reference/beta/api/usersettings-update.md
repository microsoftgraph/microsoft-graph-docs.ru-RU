---
title: Обновление параметров
description: 'Обновление свойств объекта settings. '
author: jpettere
ms.localizationpriority: medium
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 4f72bddd1d7c14dccf6a30e3a9f88a8a386620e7
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60943054"
---
# <a name="update-settings"></a>Обновление параметров

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [userSettings.](../resources/usersettings.md) Пользователи в одной организации могут иметь различные параметры в зависимости от их предпочтений или политик организации. Чтобы получить текущие параметры пользователя, см. [текущие параметры пользователя.](usersettings-get.md) 


### <a name="batch-request"></a>Пакетный запрос

Кроме того, можно отказать нескольким пользователям в доступе Delve пакетным запросом.
Дополнительные дополнительные информации см. в серии [JSON.](/graph/json-batching)

>**Важно.** Только члены группы [ролей](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) управления организацией могут обновлять несколько пользователей. 



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
|contributionToContentDiscoveryDisabled|Логический|Настройка true для отключения доступа к документам в Office Delve для пользователя. Этот параметр отражает состояние управления в [Office Delve](https://support.office.com/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).|

## <a name="example"></a>Пример 

##### <a name="request"></a>Запрос

Вот пример запроса о том, как отключать пользователя от Delve и отключить его вклад в содержимого для всей организации.

```http
PATCH https://graph.microsoft.com/beta/me/settings
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



