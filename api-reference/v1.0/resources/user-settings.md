---
title: Тип ресурса settings
description: 'Текущие параметры пользователя. '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6a1cf4deb5da03daeb9d90e03ea63fa069a0701e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033525"
---
# <a name="settings-resource-type"></a>Тип ресурса settings

Текущие параметры пользователя. Сведения о получении и обновлении параметров пользователя см. в статьях [Получение параметров](../api/user-get-settings.md) и [Обновление параметров](../api/user-update-settings.md).

Этот ресурс поддерживает:

- Проверку участия пользователя и организации пользователя в поиске содержимого.
- Включение и отключение поиска содержимого для конкретных пользователей. При этом также отключаются документы в Office Delve.

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение параметров пользователя](../api/user-get-settings.md) |[settings](../resources/user-settings.md)| Получение параметров пользователя и организации. |
|[Обновление параметров пользователя](../api/user-update-settings.md) |[settings](../resources/user-settings.md)| Обновление текущих параметров пользователя. |

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|Логический|Если задано значение true, делегированный доступ к API [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) пользователя отключен. Если задано значение true, документы в Office Delve пользователя отключены. Установка значения true влияет на релевантность содержимого, отображаемого в Office 365, например в рекомендуемых сайтах на домашней странице SharePoint и в представлении "Обнаружение" в OneDrive для бизнеса. Пользователи могут управлять этим параметром в [Office Delve](https://support.office.com/ru-RU/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout). |
|contributionToContentDiscoveryAsOrganizationDisabled|Логический|Отображает [параметр на уровне организации](https://support.office.com/ru-RU/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff), управляющий делегированным доступом к API [trending](/graph/api/resources/insights-trending?view=graph-rest-beta). Если задано значение true, у организации отсутствует доступ к Office Delve. Это влияет для всей организации на релевантность содержимого, отображаемого в Office 365, например в рекомендуемых сайтах на домашней странице SharePoint и в представлении "Обнаружение" в OneDrive для бизнеса. Этот параметр доступен только для чтения и может изменяться только администраторами в [Центре администрирования SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).|


## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
