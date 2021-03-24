---
title: Обновление mobileAppSupersedence
description: Обновление свойств объекта mobileAppSupersedence.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0397b5a029ca848fa1cb002b0930580b3978f358
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143040"
---
# <a name="update-mobileappsupersedence"></a>Обновление mobileAppSupersedence

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [mobileAppSupersedence.](../resources/intune-apps-mobileappsupersedence.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта mobileAppSupersedence.](../resources/intune-apps-mobileappsupersedence.md)

В следующей таблице показаны свойства, необходимые при создании [mobileAppSupersedence.](../resources/intune-apps-mobileappsupersedence.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|ID сущности отношений. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetId|Строка|ID приложения целевого мобильного приложения. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayName|Строка|Имя отображения целевого мобильного приложения. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayVersion|Строка|Отображаемая версия целевого мобильного приложения. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetPublisher|Строка|Издатель целевого мобильного приложения. Унаследованный от [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetType|[mobileAppRelationshipType](../resources/intune-apps-mobileapprelationshiptype.md)|Тип отношений, указывающий, является ли цель родителем или ребенком. Наследуется [от mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md). Возможные значения: `child`, `parent`.|
|supersedenceType|[mobileAppSupersedenceType](../resources/intune-apps-mobileappsupersedencetype.md)|Тип отношения supersedence между родительскими и детскими приложениями. Возможные значения: `update`, `replace`.|
|supersededAppCount|Int32|Общее количество приложений, прямо или косвенно выменимых детским приложением.|
|supersedingAppCount|Int32|Общее число приложений, прямо или косвенно выменив родительское приложение.|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
Content-type: application/json
Content-length: 375

{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "supersedenceType": "replace",
  "supersededAppCount": 2,
  "supersedingAppCount": 3
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 424

{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "id": "c0254204-4204-c025-0442-25c0044225c0",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "supersedenceType": "replace",
  "supersededAppCount": 2,
  "supersedingAppCount": 3
}
```




