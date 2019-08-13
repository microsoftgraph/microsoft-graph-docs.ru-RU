---
title: Обновление Усерекспериенцеаналитикскатегори
description: Обновление свойств объекта Усерекспериенцеаналитикскатегори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f99c4bd2090f751b0a54df6ad408cda463266605
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350490"
---
# <a name="update-userexperienceanalyticscategory"></a>Обновление Усерекспериенцеаналитикскатегори

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор категории аналитики взаимодействия с пользователем.|
|displayName|Строка|Имя категории аналитики взаимодействия с пользователем.|
|овераллскоре|Int32|Общий показатель категории аналитики взаимодействия с пользователем.|
|insights|Коллекция [усерекспериенцеаналитиксинсигхт](../resources/intune-devices-userexperienceanalyticsinsight.md)|Аналитика для категории аналитики взаимодействия с пользователем.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
Content-type: application/json
Content-length: 484

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "displayName": "Display Name value",
  "overallScore": 12,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "value": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble"
        }
      ]
    }
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 533

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "cfd28056-8056-cfd2-5680-d2cf5680d2cf",
  "displayName": "Display Name value",
  "overallScore": 12,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "value": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble"
        }
      ]
    }
  ]
}
```






