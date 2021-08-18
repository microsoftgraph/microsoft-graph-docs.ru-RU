---
title: тип ресурса macOSSoftwareUpdateAccountSummary
description: Сводный отчет об обновлении учетной записи для устройства и пользователя по программному обеспечению MacOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 57a9a7f01c44aea16e931114cade113bef2f14460bd3e9851d8989a68b348b27
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54239464"
---
# <a name="macossoftwareupdateaccountsummary-resource-type"></a>тип ресурса macOSSoftwareUpdateAccountSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводный отчет об обновлении учетной записи для устройства и пользователя по программному обеспечению MacOS

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список macOSSoftwareUpdateAccountSummaries](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-list.md)|[коллекция macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|Список свойств и связей объектов [macOSSoftwareUpdateAccountSummary.](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|
|[Получить macOSSoftwareUpdateAccountSummary](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-get.md)|[macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|Чтение свойств и связей объекта [macOSSoftwareUpdateAccountSummary.](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|
|[Создание macOSSoftwareUpdateAccountSummary](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-create.md)|[macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|Создайте новый [объект macOSSoftwareUpdateAccountSummary.](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|
|[Удаление macOSSoftwareUpdateAccountSummary](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-delete.md)|Нет|Удаляет [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md).|
|[Обновление macOSSoftwareUpdateAccountSummary](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-update.md)|[macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|Обновление свойств объекта [macOSSoftwareUpdateAccountSummary.](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|displayName|Строка|Имя отчета|
|deviceId|String|ID устройства.|
|userId|String|Идентификатор пользователя.|
|deviceName|String|Имя устройства.|
|userPrincipalName|String|Имя основного пользователя|
|osVersion|String|Версия ОС.|
|successfulUpdateCount|Int32|Количество успешных обновлений на устройстве.|
|failedUpdateCount|Int32|Количество сбойных обновлений на устройстве.|
|totalUpdateCount|Int32|Количество обновлений на устройстве.|
|lastUpdatedDateTime|DateTimeOffset|Последняя дата обновления отчета для этого устройства.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categorySummaries|[коллекция macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|Сводка обновлений по категориям.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSSoftwareUpdateAccountSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateAccountSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "deviceId": "String",
  "userId": "String",
  "deviceName": "String",
  "userPrincipalName": "String",
  "osVersion": "String",
  "successfulUpdateCount": 1024,
  "failedUpdateCount": 1024,
  "totalUpdateCount": 1024,
  "lastUpdatedDateTime": "String (timestamp)"
}
```




