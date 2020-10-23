---
title: Создание Идентитюсерфловаттрибуте
description: Создание нового объекта Идентитюсерфловаттрибуте.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 443ac0848e7ace309172dc0ca38d9a191acb9635
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742410"
---
# <a name="create-identityuserflowattribute"></a>Создание Идентитюсерфловаттрибуте

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового объекта [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Идентитюсерфлов. ReadWrite. ALL|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Приложение|Идентитюсерфлов. ReadWrite. ALL|

Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:

* Глобальный администратор
* Администратор атрибутов пользовательского процесса внешнего удостоверения

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlowAttributes
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---------------|:----------|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте представление объекта [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md)в формате JSON.

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|id|String|Идентификатор атрибута пользовательского процесса. Это автоматически создаваемый атрибут, предназначенный только для чтения.|
|displayName|String|Отображаемое имя атрибута пользовательского процесса.|
|description|String|Описание атрибута Flow User. Он отображается для пользователя во время регистрации.|
|усерфловаттрибутетипе|String|Тип атрибута пользовательского процесса. Это автоматически заданный атрибут, предназначенный только для чтения. В зависимости от типа атрибута значения этого свойства будут `builtIn` или `custom` .|
|dataType|String|Тип данных атрибута пользовательского процесса. Этот параметр нельзя изменить после создания настраиваемого атрибута пользовательского процесса. Для **DataType** поддерживаются следующие значения:<br/><ul><li>`string` : указывает, что тип данных для Идентитюсерфловаттрибуте является строкой. </li><li>`boolean` : указывает, что тип данных для Идентитюсерфловаттрибуте является логическим.</li><li>`int64` : указывает, что тип данных для Идентитюсерфловаттрибуте является целым числом.</li></ul>|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md) в тексте отклика. В случае неудачи возвращается ошибка `4xx` с подробностями.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "create_userFlowAttribute_from_userFlowAttributes"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/userFlowAttributes
Content-type: application/json

{
  "displayName": "Hobby",
  "description": "Your hobby",
  "dataType": "string",
}
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/userFlowAttributes/extension_7a95ecd9489b4fb9a45722b913c4703b_Hobby
Content-type: application/json

{
    "id": "extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby",
    "displayName": "Hobby",
    "description": "Your hobby",
    "userFlowAttributeType": "custom",
    "dataType": "string"
}
```
