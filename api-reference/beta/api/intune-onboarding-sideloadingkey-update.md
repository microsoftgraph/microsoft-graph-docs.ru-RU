---
title: Обновление sideLoadingKey
description: Обновление свойств объекта sideLoadingKey.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 65ae9cfcb7fd2d66c8b56108929a284f26d840fa
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152672"
---
# <a name="update-sideloadingkey"></a>Обновление sideLoadingKey

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [sideLoadingKey.](../resources/intune-onboarding-sideloadingkey.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта sideLoadingKey.](../resources/intune-onboarding-sideloadingkey.md)

В следующей таблице показаны свойства, необходимые при создании [sideLoadingKey.](../resources/intune-onboarding-sideloadingkey.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный ID side Loading Key.|
|value|String|Ключевое значение side Loading — это значение 5x5, разделенное hiphens.|
|displayName|Строка|Имя клавиши боковой загрузки, отображаемой администраторам ITPro.|
|description|Строка|Описание клавиши боковой загрузки, отображаемой администраторам ITPro..|
|totalActivation|Int32|Полная активация клавиши боковой загрузки, отображаемая администраторам ITPro.|
|lastUpdatedDateTime|Строка|Клавиша side Loading Last Updated Date, отображаемая администраторам ITPro.|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и `200 OK` обновленный [объект sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
Content-type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```




