---
title: Тип ресурса userSettings
description: 'Параметры текущего пользователя для поиска контента. '
author: krbain
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 81391c38f2577fd3f60c57fa40f9671ae710c2a2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057775"
---
# <a name="usersettings-resource-type"></a>Тип ресурса userSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры, представляющие предпочтения пользователя для [региональных языковых стандартов и языков](../resources/regionalandlanguagesettings.md), для [планирования расписаний](../resources/shiftpreferences.md), а также для [анализа и обнаружения контента](../resources/officegraphinsights.md).

Управление настройками на основе языкового стандарта пользователя: 
  - Определение языка и региональных форматов, предпочитаемых пользователем для просмотра приложений.
  - Обновление языков и региональных параметров форматирования пользователя.

Управление настройками рабочей смены пользователя: 
  - Проверка того, можно ли назначить пользователя для смены по расписанию.
  - Обновление предпочтений пользователя при смене.
  
Включение обнаружения контента и аналитической информации, ориентированной на документы:
  - Проверку участия пользователя и организации пользователя в поиске содержимого.
  - Включение и отключение поиска содержимого для конкретных пользователей. При этом также отключаются документы в Office Delve.

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
|contributionToContentDiscoveryDisabled|Логический|Если задано значение true, делегированный доступ к API [trending](insights-trending.md) пользователя отключен. Если задано значение true, документы в Office Delve пользователя отключены. Если задано значение true, то релевантность содержимого, отображаемого в Microsoft 365, например в разделе Рекомендуемые сайты в SharePoint Home и представление "Обнаружение" в OneDrive для бизнеса влияет. Пользователи могут управлять этим параметром в [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout). |
|contributionToContentDiscoveryAsOrganizationDisabled|Логический|Отображает [параметр на уровне организации](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff), управляющий делегированным доступом к API [trending](insights-trending.md). Если задано значение true, у организации отсутствует доступ к Office Delve. Релевантность содержимого, отображаемого в Microsoft 365, например в разделе Рекомендуемые сайты в SharePoint Home, а представление обнаружения в OneDrive для бизнеса влияет на всю организацию. Этот параметр доступен только для чтения и может изменяться только администраторами в [Центре администрирования SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).|

## <a name="relationships"></a>Связи

| Связь | Тип | Описание |
|:---------------|:--------|:----------|
|шифтпреференцес|[шифтпреференцес](shiftpreferences.md)| Настройки смены для пользователя. |
|регионаландлангуажесеттингс|[регионаландлангуажесеттингс](regionalandlanguagesettings.md)| Предпочтения пользователя для языков, региональных стандартов и форматирования даты и времени. |

## <a name="json-representation"></a>Представление в формате JSON

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


