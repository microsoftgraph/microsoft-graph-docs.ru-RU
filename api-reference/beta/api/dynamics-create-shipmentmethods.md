---
title: Создание Шипментмесодс
description: Создает объект метода отгрузки в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 8b33d044549a67ce27bb160db382e06bbcf73b9d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431255"
---
# <a name="create-shipmentmethods"></a>Создание Шипментмесодс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте объект метода отгрузки в Dynamics 365 Business Central.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения |Разрешения (в порядке повышения привилегий)|
|:---------------|:------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Financials.ReadWrite.All |
|Делегированная учетная запись (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
```
POST /financials/companies/{id}/shipmentMethods
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов

|Заголовок         |Значение                     |
|---------------|--------------------------|
|Авторизация  |Bearer {токен}. Обязательный. |
|Content-Type   |application/json          |

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта **шипментмесодс** в формате JSON.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **шипментмесодс** в тексте отклика.

## <a name="example"></a>Пример

**Запрос**

Ниже приведен пример запроса.

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/shipmentMethods
Content-type: application/json

{
  "code": "PICKUP",
  "displayName": "Pickup at Location"  
}
```

**Отклик**

Ниже приведен пример отклика. 

> **Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "PICKUP",
  "displayName": "Pickup at Location",
  "lastModifiedDateTime": "2017-03-15T02:20:57.09Z"
}

```
