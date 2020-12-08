---
title: Создание Усераттрибутеассигнментс
description: Создание нового объекта Идентитюсерфловаттрибутеассигнмент.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8c838dfee57e264d7cca61ac5e10ec98a46f7330
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581351"
---
# <a name="create-userattributeassignments"></a>Создание Усераттрибутеассигнментс

Пространство имен: microsoft.graph

Создание нового объекта Идентитюсерфловаттрибутеассигнмент в [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).

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
POST /identity/b2cUserFlows/{id}/userAttributeAssignments
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [идентитюсерфловаттрибутеассигнмент](../resources/identityuserflowattributeassignment.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [идентитюсерфловаттрибутеассигнмент](../resources/identityuserflowattributeassignment.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя Идентитюсерфловаттрибуте в пользовательском движении.|
|Переключатель|Логический|Определяет, является ли Идентитюсерфловаттрибуте необязательным. `true` означает, что пользователю не нужно указывать значение. `false` означает, что пользователь не может выполнить вход, не указывая значение.|
|рекуиресверификатион|Логический|Определяет, требуется ли для Идентитюсерфловаттрибуте проверка. Используется только для проверки номера телефона пользователя или адреса электронной почты.|
|усераттрибутевалуес|Коллекция [усераттрибутевалуеситем](../resources/userattributevaluesitem.md)|Параметры ввода для атрибута Flow User. Применяется только в том случае, если для Усеринпуттипе задано значение `radioSingleSelect` , `dropdownSingleSelect` или `checkboxMultiSelect` .|
|усеринпуттипе|идентитюсерфловаттрибутеинпуттипе|Тип входных данных для атрибута Flow User. Возможные значения: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.|
|усераттрибуте|[идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md)|Идентификатор атрибута пользовательского процесса, включаемый в назначение пользовательского процесса.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [идентитюсерфловаттрибутеассигнмент](../resources/identityuserflowattributeassignment.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_identityuserflowattributeassignment_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Consumer/userAttributeAssignments
Content-Type: application/json

{
    "isOptional": false,
    "requiresVerification": false,
    "userInputType": "TextBox",
    "displayName": "Shoe size",
    "userAttributeValues": [],
    "userAttribute": {
        "id": "extension_guid_shoeSize"
    }
}
```

### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment"
}
-->

``` http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2xUserFlows/B2C_1_Consumer/userAttributeAssignments/extension_guid_shoeSize
Content-Type: application/json

{
    "id": "extension_guid_shoeSize",
    "isOptional": false,
    "requiresVerification": false,
    "userInputType": "TextBox",
    "displayName": "Shoe size",
    "userAttributeValues": []
}
```
