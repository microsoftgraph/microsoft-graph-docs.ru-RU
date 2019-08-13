---
title: Тип ресурса Мобилеконтаинедапп
description: Абстрактный класс, представляющий вложенное приложение в mobileApp, работающее в виде пакета.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4f0c20b73c753ea4d51e18469f97841b02e01e83
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331779"
---
# <a name="mobilecontainedapp-resource-type"></a>Тип ресурса Мобилеконтаинедапп

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Абстрактный класс, представляющий вложенное приложение в mobileApp, работающее в виде пакета.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Мобилеконтаинедаппс](../api/intune-apps-mobilecontainedapp-list.md)|Коллекция [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)|Список свойств и связей объектов [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md) .|
|[Получение Мобилеконтаинедапп](../api/intune-apps-mobilecontainedapp-get.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md);|Чтение свойств и связей объекта [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|

## <a name="relationships"></a>Отношения
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



