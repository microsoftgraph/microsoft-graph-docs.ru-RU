---
title: Тип ресурса learningProvider
description: Представляет сущность, содержащую сведения о поставщике обучения.
author: malabikaroy
ms.localizationpriority: medium
ms.prod: employee-learning
doc_type: resourcePageType
ms.openlocfilehash: eb68ab517f0df414202ac8d676838fb3161472cf
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883394"
---
# <a name="learningprovider-resource-type"></a>Тип ресурса learningProvider

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сущность, содержащую сведения о поставщике обучения в обучении Viva.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов learningProvider](../api/employeeexperience-list-learningproviders.md)|[Коллекция learningProvider](../resources/learningprovider.md)|Получение списка ресурсов [learningProvider](../resources/learningprovider.md), зарегистрированных в Viva Обучение клиента.|
|[Создание learningProvider](../api/employeeexperience-post-learningproviders.md)|[learningProvider](../resources/learningprovider.md)|Создайте объект [learningProvider](../resources/learningprovider.md) и зарегистрируйте его в Viva Обучение с использованием указанного отображаемого имени и логотипов для разных тем.|
|[Получение learningProvider](../api/learningprovider-get.md)|[learningProvider](../resources/learningprovider.md)|Чтение свойств и связей объекта [learningProvider](../resources/learningprovider.md) .|
|[Обновление learningProvider](../api/learningprovider-update.md)|[learningProvider](../resources/learningprovider.md)|Обновление свойств объекта [learningProvider](../resources/learningprovider.md) .|
|[Удаление learningProvider](../api/employeeexperience-delete-learningproviders.md)|Нет|Удалите [ресурс learningProvider](../resources/learningprovider.md) и удалите его регистрацию в Viva Обучение клиента.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя, отображаемое в Viva Обучение. Обязательный.|
|id|Строка|Уникальный идентификатор поставщика обучения. Обязательный.|
|isEnabled|Boolean|Состояние поставщика. Необязательный элемент.|
|loginWebUrl|String|URL-адрес проверки подлинности для доступа к курсам для поставщика. Необязательный элемент.|
|longLogoWebUrlForDarkTheme|String|Длинный URL-адрес логотипа для темного режима, который должен быть общедоступным изображением. Это изображение будет сохранено в хранилище BLOB-объектов Viva Обучение для отрисовки в Viva Обучение приложения. Обязательный.|
|longLogoWebUrlForLightTheme|String|Длинный URL-адрес логотипа для светлого режима, который должен быть общедоступным изображением. Это изображение будет сохранено в хранилище BLOB-объектов Viva Обучение для отрисовки в Viva Обучение приложения. Обязательный.|
|squareLogoWebUrlForDarkTheme|String|URL-адрес квадратного логотипа для темного режима, который должен быть общедоступным изображением. Это изображение будет сохранено в хранилище BLOB-объектов Viva Обучение для отрисовки в Viva Обучение приложения. Обязательный.|
|squareLogoWebUrlForLightTheme|String|URL-адрес квадратного логотипа для режима освещения, который должен быть общедоступным изображением. Это изображение будет сохранено в хранилище BLOB-объектов Viva Обучение для отрисовки в Viva Обучение приложения. Обязательный.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|learningContents|[Коллекция learningContent](../resources/learningcontent.md)|Изучение элементов каталога для поставщика.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.learningProvider",
  "openType": false
}
-->
``` json
{
    "@odata.type": "#microsoft.graph.learningProvider",
    "displayName": "String",
    "id": "String (identifier)",
    "isEnabled": "Boolean",
    "loginWebUrl": "String",
    "longLogoWebUrlForDarkTheme": "String",
    "longLogoWebUrlForLightTheme": "String",
    "squareLogoWebUrlForDarkTheme": "String",
    "squareLogoWebUrlForLightTheme": "String"
}
```

