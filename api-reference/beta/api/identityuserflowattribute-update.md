---
title: Обновление Идентитюсерфловаттрибуте
description: Обновление свойств объекта Идентитюсерфловаттрибуте.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fe74ffc6b360c2f83b917e9852a42faa6e193955
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742373"
---
# <a name="update-identityuserflowattribute"></a>Обновление Идентитюсерфловаттрибуте

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md) . Можно обновлять только настраиваемые атрибуты пользовательского процесса.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Идентитюсерфлов. ReadWrite. ALL|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Приложение| Идентитюсерфлов. ReadWrite. ALL|

Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:

* Глобальный администратор
* Внешний идентификатор пользователя Администратор атрибутов пользовательского процесса

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /userFlowAttributes/{id}
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---------------|:----------|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите объект JSON с одним или несколькими свойствами, которые необходимо обновить для объекта [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md) .

>**Примечание:** Можно обновить только свойство **Description** .

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|description|String|Описание атрибута Flow User. Он отображается для пользователя во время регистрации.|

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. В случае неудачи возвращается ошибка `4xx` с подробностями.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "update_userFlowAttributes"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/userFlowAttributes/extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby
Content-type: application/json

{
  "description": "Your new hobby"
}
```

### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
