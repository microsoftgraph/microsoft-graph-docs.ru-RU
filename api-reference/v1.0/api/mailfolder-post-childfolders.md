---
title: Создание объекта MailFolder
description: С помощью этого API можно создать дочернюю папку почты.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: bf078e34f216dde5a3daf3bcf0cecd27517e7da7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565417"
---
# <a name="create-mailfolder"></a>Создание объекта MailFolder

С помощью этого API можно создать дочернюю папку почты.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:----------------|:--------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Mail.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Mail.ReadWrite    |
|Для приложений | Mail.ReadWrite |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

Укажите родительскую папку в URL-АДРЕСе запроса как идентификатор папки или известное имя папки. Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).

## <a name="request-headers"></a>Заголовки запросов

| Заголовок | Значение |
|:-------|:------|
| Авторизация | `Bearer {token}`. Обязательный параметр. |
| Content-Type | `application/json`. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами. **DisplayName** это единственное свойство для записи объекта [mailFolder](../resources/mailfolder.md) .

| Параметр | Тип | Описание |
|:----------|:-----|:------------|
|displayName|String|Отображаемое имя новой папки.|

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод `201 Created` возвращает код отклика и ресурс [mailFolder](../resources/mailfolder.md) в тексте отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика.

> **Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
