---
title: Обновление educationAssignmentSettings
description: Обновление свойств объекта educationAssignmentSettings.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0475f49b400b12e8716fcb2ba122c99cf46f4b1e
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034351"
---
# <a name="update-educationassignmentsettings"></a>Обновление educationAssignmentSettings
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [educationAssignmentSettings.](../resources/educationassignmentsettings.md) Только преподаватели могут обновлять эти параметры.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /education/classes/{id}/assignmentSettings
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса укажу представление объекта [educationAssignmentSettings](../resources/educationassignmentsettings.md) в JSON.

В следующей таблице показаны свойства, необходимые при обновлении [объекта educationAssignmentSettings.](../resources/educationassignmentsettings.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|submissionAnimationDisabled|Логический|Указывает, будет ли показана анимация поозднения. Значение `true` указывает, что анимация не будет показана. Значение по умолчанию: `false`.|



## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [educationAssignmentSettings](../resources/educationassignmentsettings.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "update_educationassignmentsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/education/classes/{id}/assignmentSettings
Content-Type: application/json
Content-length: 114

{
  "submissionAnimationDisabled": true
}
```


### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "submissionAnimationDisabled": true
}
```

