---
title: Тип ресурса userSettings
description: 'Параметры текущего пользователя для поиска контента. '
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 12c75691b5b0515fbf8ef49b54ce1e4a0b806c2c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761774"
---
# <a name="usersettings-resource-type"></a>Тип ресурса userSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры, которые представляют предпочтения пользователя для регионального языка и [языков,](../resources/regionalandlanguagesettings.md)для планирования [смены,](../resources/shiftpreferences.md)а также для анализа и [обнаружения контента.](../resources/officegraphinsights.md)

Управление предпочтениями на основе локального пользователя: 
  - Определение языка и регионального форматирования, с помощью чего пользователь предпочитает просматривать приложения.
  - Обновление языковых и региональных предпочтений форматирования пользователя.

Управление предпочтениями смены работы пользователя: 
  - Проверка того, можно ли пользователю назначены изменения в расписании.
  - Обновление личных предпочтений пользователя.
  
Включить обнаружение контента и документов, ориентированных на анализ:
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
|contributionToContentDiscoveryDisabled|Логический|Если задано значение true, делегированный доступ к API [trending](insights-trending.md) пользователя отключен. Если задано значение true, документы в Office Delve пользователя отключены. Установка значения true влияет на релевантность содержимого, отображаемого в Microsoft 365, например в рекомендуемых сайтах на домашней странице SharePoint и в представлении "Обнаружение" в OneDrive для бизнеса. Пользователи могут управлять этим параметром в [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout). |
|contributionToContentDiscoveryAsOrganizationDisabled|Логический|Отображает [параметр на уровне организации](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff), управляющий делегированным доступом к API [trending](insights-trending.md). Если задано значение true, у организации отсутствует доступ к Office Delve. Это влияет на релевантность содержимого, отображаемого в Microsoft 365 для всей организации, например в рекомендуемых сайтах на домашней странице SharePoint и в представлении "Обнаружение" в OneDrive для бизнеса. Этот параметр доступен только для чтения и может изменяться только администраторами в [Центре администрирования SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).|

## <a name="relationships"></a>Отношения

| Связь | Тип | Описание |
|:---------------|:--------|:----------|
|shiftPreferences|[shiftPreferences](shiftpreferences.md)| Параметры переноса для пользователя. |
|regionalAndLanguageSettings|[regionalAndLanguageSettings](regionalandlanguagesettings.md)| Предпочтения пользователя для языков, регионального языка и форматирования даты и времени. |

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


