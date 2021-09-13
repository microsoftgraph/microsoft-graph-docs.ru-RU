---
title: тип ресурса mobileContainedApp
description: Абстрактный класс, представляю содержащийся в приложении mobileApp, действующий в качестве пакета.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 281100ad8f91bc8872cba5228a1d6a9a24a42167
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075846"
---
# <a name="mobilecontainedapp-resource-type"></a>тип ресурса mobileContainedApp

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Абстрактный класс, представляю содержащийся в приложении mobileApp, действующий в качестве пакета.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список mobileContainedApps](../api/intune-apps-mobilecontainedapp-list.md)|[коллекция mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|Список свойств и связей объектов [mobileContainedApp.](../resources/intune-apps-mobilecontainedapp.md)|
|[Get mobileContainedApp](../api/intune-apps-mobilecontainedapp-get.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|Чтение свойств и связей объекта [mobileContainedApp.](../resources/intune-apps-mobilecontainedapp.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileContainedApp",
  "id": "String (identifier)"
}
```



