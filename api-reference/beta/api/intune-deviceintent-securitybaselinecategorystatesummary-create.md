---
title: Создание securityBaselineCategoryStateSummary
description: Создайте новый объект securityBaselineCategoryStateSummary.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5ad7b43b86a99464ae73794bd1067b08a6164d4b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59103013"
---
# <a name="create-securitybaselinecategorystatesummary"></a>Создание securityBaselineCategoryStateSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте новый [объект securityBaselineCategoryStateSummary.](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)

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
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса укажи представление JSON для объекта securityBaselineCategoryStateSummary.

В следующей таблице показаны свойства, необходимые при создании securityBaselineCategoryStateSummary.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта. Унаследованный от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|secureCount|Int32|Количество защищенных устройств, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|notSecureCount|Int32|Количество не защищенных устройств, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|unknownCount|Int32|Количество неизвестных устройств, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|errorCount|Int32|Количество устройств с ошибками, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|conflictCount|Int32|Количество конфликтных устройств, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|notApplicableCount|Int32|Количество не применимых устройств, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|displayName|String|Имя категории|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и объект `201 Created` [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
Content-type: application/json
Content-length: 261

{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2,
  "displayName": "Display Name value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "id": "7a650997-0997-7a65-9709-657a9709657a",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2,
  "displayName": "Display Name value"
}
```



