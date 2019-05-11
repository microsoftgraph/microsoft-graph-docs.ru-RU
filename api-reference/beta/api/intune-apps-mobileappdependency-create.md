---
title: Создание Мобилеаппдепенденци
description: Создание нового объекта Мобилеаппдепенденци.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a272a9c39262b6dd14c8d118f8c50e615d92583
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935149"
---
# <a name="create-mobileappdependency"></a>Создание Мобилеаппдепенденци

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта Мобилеаппдепенденци в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Мобилеаппдепенденци.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор сущности отношения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)|
|targetId|Строка|Идентификатор приложения целевого дочернего мобильного приложения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)|
|Таржетдисплайнаме|Строка|Отображаемое имя целевого дочернего мобильного приложения. Наследуется от [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)|
|Депенденцитипе|[Мобилеаппдепенденцитипе](../resources/intune-apps-mobileappdependencytype.md)|Тип отношения зависимости между родительским и дочерним приложениями. Возможные значения: `detect`, `autoInstall`.|
|Депендентаппкаунт|Int32|Общее количество зависимостей для дочернего приложения.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```




