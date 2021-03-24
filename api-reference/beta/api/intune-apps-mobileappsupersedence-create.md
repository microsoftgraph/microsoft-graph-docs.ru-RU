---
title: Создание mobileAppSupersedence
description: Создание нового объекта mobileAppSupersedence.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02410619b871c00b92bfacd8df09ff221baff68e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143096"
---
# <a name="create-mobileappsupersedence"></a>Создание mobileAppSupersedence

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта mobileAppSupersedence.](../resources/intune-apps-mobileappsupersedence.md)

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
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта mobileAppSupersedence.

В следующей таблице показаны свойства, необходимые при создании mobileAppSupersedence.

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
В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
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
HTTP/1.1 201 Created
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




