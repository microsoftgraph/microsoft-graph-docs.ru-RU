---
title: Обновление Идентитюсерфловаттрибутеассигнмент
description: Обновление свойств объекта Усераттрибутеассигнментс.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2b9b5e39cd8d7462b678608ae74727eacdf101cb
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581423"
---
# <a name="update-identityuserflowattributeassignment"></a>Обновление Идентитюсерфловаттрибутеассигнмент

Пространство имен: microsoft.graph

Обновление свойств объекта Идентитюсерфловаттрибутеассигнмент.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|Идентитюсерфлов. ReadWrite. ALL|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|Идентитюсерфлов. ReadWrite. ALL|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
PATCH /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [идентитюсерфловаттрибутеассигнмент](../resources/identityuserflowattributeassignment.md) в формате JSON.

В следующей таблице приведены свойства, доступные для обновления в [идентитюсерфловаттрибутеассигнмент](../resources/identityuserflowattributeassignment.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя Идентитюсерфловаттрибуте в пользовательском движении.|
|Переключатель|Логический|Определяет, является ли Идентитюсерфловаттрибуте необязательным. `true` означает, что пользователю не нужно указывать значение. `false` Указывает, что пользователь не может выполнить вход, не предоставляя значение.|
|рекуиресверификатион|Логический|Определяет, требуется ли для Идентитюсерфловаттрибуте проверка. Используется только для проверки номера телефона пользователя или адреса электронной почты.|
|усераттрибутевалуес|Коллекция [усераттрибутевалуеситем](../resources/userattributevaluesitem.md)|Параметры ввода для атрибута Flow User. Применяется только в том случае, если для Усеринпуттипе задано значение `radioSingleSelect` , `dropdownSingleSelect` или `checkboxMultiSelect` .|
|усеринпуттипе|идентитюсерфловаттрибутеинпуттипе|Тип входных данных для атрибута Flow User. Возможные значения: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [идентитюсерфловаттрибутеассигнмент](../resources/identityuserflowattributeassignment.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "update_userattributeassignments"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/{id}
Content-Type: application/json

{
  "userInputType": "textBox"
}
```

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
