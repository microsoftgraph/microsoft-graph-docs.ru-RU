---
title: Обновление securityBaselineStateSummary
description: Обновление свойств объекта securityBaselineStateSummary.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ecf22417b4c802e446167af5298fef63113bd53a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030888"
---
# <a name="update-securitybaselinestatesummary"></a>Обновление securityBaselineStateSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [securityBaselineStateSummary.](../resources/intune-deviceintent-securitybaselinestatesummary.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта securityBaselineStateSummary.](../resources/intune-deviceintent-securitybaselinestatesummary.md)

В следующей таблице показаны свойства, необходимые при создании [securityBaselineStateSummary.](../resources/intune-deviceintent-securitybaselinestatesummary.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта.|
|secureCount|Int32|Количество защищенных устройств|
|notSecureCount|Int32|Число небезопасных устройств|
|unknownCount|Int32|Количество неизвестных устройств.|
|errorCount|Int32|Количество устройств с ошибками.|
|conflictCount|Int32|Количество конфликтующих устройств.|
|notApplicableCount|Int32|Количество неприменимых устройств.|



## <a name="response"></a>Ответ
В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
Content-type: application/json
Content-length: 213

{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 262

{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "id": "a4da796f-796f-a4da-6f79-daa46f79daa4",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2
}
```



