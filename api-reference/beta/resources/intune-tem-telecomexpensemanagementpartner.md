---
title: Тип ресурса telecomExpenseManagementPartner
description: Ресурсы telecomExpenseManagementPartner представляют метаданные и сведения о состоянии определенной службы TEM. После подключения партнера к вашей организации вы можете разрешить или запретить ему включать и отключать функции TEM.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dede7807703bbd68dd965d9690904520b7a83d14
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523417"
---
# <a name="telecomexpensemanagementpartner-resource-type"></a>Тип ресурса telecomExpenseManagementPartner

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурсы telecomExpenseManagementPartner представляют метаданные и сведения о состоянии определенной службы TEM. После подключения партнера к вашей организации вы можете разрешить или запретить ему включать и отключать функции TEM.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов telecomExpenseManagementPartners](../api/intune-tem-telecomexpensemanagementpartner-list.md)|Коллекция [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Список свойств и связей объектов [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).|
|[Получение объекта telecomExpenseManagementPartner](../api/intune-tem-telecomexpensemanagementpartner-get.md)|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md);|Чтение свойств и связей объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).|
|[Создание объекта telecomExpenseManagementPartner](../api/intune-tem-telecomexpensemanagementpartner-create.md)|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md);|Создание объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).|
|[Удаление объекта telecomExpenseManagementPartner](../api/intune-tem-telecomexpensemanagementpartner-delete.md)|Нет|Удаляет объект [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).|
|[Обновление объекта telecomExpenseManagementPartner](../api/intune-tem-telecomexpensemanagementpartner-update.md)|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Обновление свойств объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор партнера TEM.|
|displayName|Строка|Отображаемое имя партнера TEM.|
|url|String|URL-адрес административной панели управления партнера TEM, где администратор может настроить службу TEM.|
|appAuthorized|Boolean|Определяет, разрешен ли доступ к Intune партнерскому приложению AAD.|
|enabled|Boolean|Определяет, включено или отключено сейчас подключение Intune к службе TEM.|
|lastConnectionDateTime|DateTimeOffset|Метка времени последнего запроса, отправленного службе Intune партнером TEM.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.telecomExpenseManagementPartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "String (identifier)",
  "displayName": "String",
  "url": "String",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "String (timestamp)"
}
```



