---
title: Обновление параметров
description: 'Обновление свойств объекта settings. '
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 0b20225fe22ede9cf0226a3fd1b4c3332922bf6c
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582060"
---
# <a name="update-settings"></a>Обновление параметров

Пространство имен: microsoft.graph

Обновление свойств объекта [усерсеттингс](../resources/usersettings.md) . Пользователи в одной организации могут иметь различные параметры в зависимости от их предпочтения или политики Организации. Чтобы получить текущие параметры пользователя, просмотрите [параметры текущей учетной записи пользователя](usersettings-get.md). 

### <a name="batch-request"></a>Пакетный запрос

Кроме того, можно отказаться от использования нескольких пользователей из delve и отказаться от их вклада в релевантность содержимого для всей Организации с помощью пакетного запроса.
Для получения дополнительных сведений см [Пакетная обработка JSON](/graph/json-batching).

>**Важно!** только члены группы ролей " [Управление организацией](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) " могут обновлять нескольких пользователей. 



## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированное (рабочая или учебная учетная запись) | User. ReadWrite, User. ReadWrite. ALL   |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается.    |
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
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|Логический|Установите значение true, чтобы запретить представителю доступ к API [тенденций](/graph/api/resources/insights-trending?view=graph-rest-1.0) и отключить доступ к документам в Office delve для пользователя. Значение true также влияет на релевантность контента, отображаемого в Microsoft 365 — например, Рекомендуемые сайты в SharePoint Home и представление обнаружение в OneDrive для бизнеса содержат менее релевантные результаты. Этот параметр отражает состояние элемента управления в [Office delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).|

## <a name="example"></a>Пример 

##### <a name="request"></a>Запрос

Ниже приведен пример запроса на отказаться от участия пользователя в delve и отказаться от его участия в релевантности контента для всей Организации.

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a>Отклик

Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```