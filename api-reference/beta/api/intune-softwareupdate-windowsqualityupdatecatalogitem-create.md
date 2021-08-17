---
title: Создание windowsQualityUpdateCatalogItem
description: Создайте новый объект WindowsQualityUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d7a204488503a5df0b19d6dfc7e6ca9ba7a960a03a70de863f7a597dea8ad9c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54122931"
---
# <a name="create-windowsqualityupdatecatalogitem"></a>Создание windowsQualityUpdateCatalogItem

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте [новый объект WindowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsUpdateCatalogItems
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта WindowsQualityUpdateCatalogItem.

В следующей таблице показаны свойства, необходимые при создании windowsQualityUpdateCatalogItem.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID элемента каталога. Унаследованный от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|displayName|Строка|Имя отображения элемента каталога. Унаследованный от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|releaseDateTime|DateTimeOffset|Дата выпуска элемента каталога, наследуемого [из windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|endOfSupportDate|DateTimeOffset|Последняя поддерживаемая дата для элемента каталога, наследуемого [из windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|kbArticleId|Строка|ID статьи базы знаний|
|classification|[windowsQualityUpdateClassification](../resources/intune-softwareupdate-windowsqualityupdateclassification.md)|Классификация обновления качества. Возможные значения: `all`, `security`, `nonSecurity`.|
|isExpeditable|Логический|Флаг, указывающий, имеет ли обновление право на ускорение|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и `201 Created` [объект WindowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems
Content-type: application/json
Content-length: 332

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00",
  "kbArticleId": "Kb Article Id value",
  "classification": "security",
  "isExpeditable": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 381

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
  "id": "8eb831ba-31ba-8eb8-ba31-b88eba31b88e",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00",
  "kbArticleId": "Kb Article Id value",
  "classification": "security",
  "isExpeditable": true
}
```




