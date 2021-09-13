---
title: Создание deviceManagementStringSettingInstance
description: Создание нового объекта deviceManagementStringSettingInstance.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b1b1629d79ae86cd921581603f92c18be2cc0746
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59116787"
---
# <a name="create-devicemanagementstringsettinginstance"></a>Создание deviceManagementStringSettingInstance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта deviceManagementStringSettingInstance.](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/settings
POST /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта deviceManagementStringSettingInstance.

В следующей таблице показаны свойства, необходимые при создании устройстваManagementStringSettingInstance.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID экземпляра параметра, унаследованный от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|definitionId|String|ID определения параметра для этого экземпляра, унаследованный от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|valueJson|String|Представление JSON значения, унаследованной от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|value|String|Значение строки|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": "Value value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "id": "fef30638-0638-fef3-3806-f3fe3806f3fe",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": "Value value"
}
```



