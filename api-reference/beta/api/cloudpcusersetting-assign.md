---
title: 'cloudPcUserSetting: назначение'
description: Назначение параметров пользователя облачного КОМПЬЮТЕРА группам пользователей.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 66da3f668cc25807ece4a63e51dabe3f5436cf7d
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082092"
---
# <a name="cloudpcusersetting-assign"></a>cloudPcUserSetting: назначение

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Назначение [cloudPcUserSetting группам](../resources/cloudpcusersetting.md) пользователей.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|CloudPC.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|CloudPC.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/userSettings/{id}/assign
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В корпусе запроса поставляем представление JSON объекта [cloudPcUserSettingAssignment.](../resources/cloudpcusersettingassignment.md)

|Параметр|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md) | Коллекция пользовательских облачных КОМПЬЮТЕРов, устанавливая ресурсы, которые должны быть назначены соответствующей целевой группе. В Microsoft 365 поддерживаются только группы и группы безопасности в Azure AD. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "cloudpcusersetting_assign"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff/assign
Content-Type: application/json
Content-length: 254

{
  "assignments": [
    {
      "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
      "target":{
        "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
        "groupId":"64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
        }
    }
  ]
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
