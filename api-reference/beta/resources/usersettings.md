---
title: Тип ресурса userSettings
description: 'Параметры текущего пользователя для поиска контента. '
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: a16ab96bb04f6d7dfc4f9ceff29f49dc7d348d23
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108875"
---
# <a name="usersettings-resource-type"></a>Тип ресурса userSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры, которые представляют предпочтения пользователя для регионального языка и [языков,](../resources/regionalandlanguagesettings.md)для планирования [смены,](../resources/shiftpreferences.md)для Delve и для [элементов.](../resources/officegraphinsights.md)

Управление предпочтениями на основе локального пользователя: 
  - Определение языка и регионального форматирования, с помощью чего пользователь предпочитает просматривать приложения.
  - Обновление языковых и региональных предпочтений форматирования пользователя.

Управление предпочтениями смены работы пользователя: 
  - Проверка того, можно ли пользователю назначены изменения в расписании.
  - Обновление личных предпочтений пользователя.
  
Управление Delve доступностью:
  - Проверка доступа пользователя и организации пользователя к Office Delve.
  - Отключение или включение документов в Office Delve для определенных пользователей. 

Настройка видимости [itemInsights и](../resources/iteminsights.md) [собраний.](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) ItemInsights являются производными между пользователями и другими элементами (например, документами или сайтами) в Microsoft 365:
  - Проверка включения элементов и часов собраний пользователя.
  - Отключение или включение данных о элементах и часах собраний для конкретного пользователя.

Сведения о получении и обновлении параметров пользователя см. в статьях [Получение параметров](../api/usersettings-get.md) и [Обновление параметров](../api/usersettings-update.md).

> [!NOTE]
> Эта конечная точка работает только с пользователями. Вы не можете использовать эту конечную точку с контактами.

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение параметров пользователя](../api/usersettings-get.md) |[userSettings](../resources/usersettings.md)| Получение параметров пользователя и организации. |
|[Обновление параметров пользователя](../api/usersettings-update.md) |[userSettings](../resources/usersettings.md)| Обновление текущих параметров пользователя. |

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|Логический|Если задано значение true, документы в Office Delve пользователя отключены. Пользователи могут управлять этим параметром в [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout). |
|contributionToContentDiscoveryAsOrganizationDisabled|Логический|Отражает параметр [уровня Office Delve организации.](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) Если задано значение true, у организации отсутствует доступ к Office Delve. Этот параметр доступен только для чтения и может изменяться только администраторами в [Центре администрирования SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).|

## <a name="relationships"></a>Отношения

| Связь | Тип | Описание |
|:---------------|:--------|:----------|
|shiftPreferences|[shiftPreferences](shiftpreferences.md)| Параметры переноса для пользователя. |
|regionalAndLanguageSettings|[regionalAndLanguageSettings](regionalandlanguagesettings.md)| Предпочтения пользователя для языков, регионального языка и форматирования даты и времени. |
|itemInsights|[userInsightsSettings](userinsightssettings.md)| Параметры пользователя для видимости информации о часах собраний и сведения, полученные между пользователем и другими элементами в Microsoft 365, например документами или сайтами. [Получите userInsightsSettings через](../api/userinsightssettings-get.md) это свойство навигации. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userSettings",
  "baseType": "microsoft.graph.entity"
}-->
```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```


