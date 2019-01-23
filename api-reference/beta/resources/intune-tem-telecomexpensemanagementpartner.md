---
title: Тип ресурса telecomExpenseManagementPartner
description: Ресурсы telecomExpenseManagementPartner представляют метаданные и сведения о состоянии определенной службы TEM. После подключения партнера к вашей организации вы можете разрешить или запретить ему включать и отключать функции TEM.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e1d148366a9ff67b643bad37e6aef5ed67653d1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401854"
---
# <a name="telecomexpensemanagementpartner-resource-type"></a>Тип ресурса telecomExpenseManagementPartner

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурсы telecomExpenseManagementPartner представляют метаданные и сведения о состоянии определенной службы TEM. После подключения партнера к вашей организации вы можете разрешить или запретить ему включать и отключать функции TEM.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов telecomExpenseManagementPartners](../api/intune-tem-telecomexpensemanagementpartner-list.md)|Коллекция [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Список свойств и связей объектов [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).|
|[Получение объекта telecomExpenseManagementPartner](../api/intune-tem-telecomexpensemanagementpartner-get.md)|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Чтение свойств и связей объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).|
|[Создание объекта telecomExpenseManagementPartner](../api/intune-tem-telecomexpensemanagementpartner-create.md)|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Создание объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).|
|[Удаление объекта telecomExpenseManagementPartner](../api/intune-tem-telecomexpensemanagementpartner-delete.md)|Нет|Удаляет объект [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).|
|[Обновление объекта telecomExpenseManagementPartner](../api/intune-tem-telecomexpensemanagementpartner-update.md)|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Обновление свойств объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор партнера TEM.|
|displayName|String|Отображаемое имя партнера TEM.|
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




