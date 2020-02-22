---
title: Интеграция решений по обеспечению безопасности с помощью Microsoft Graph Security API
description: Все возможности, описанные в этой статье, позволяют подключаться к Microsoft Graph Security API. Эти возможности позволяют работать с данными в едином формате в разных поддерживаемых решениях поставщиков безопасности партнеров и Майкрософт с помощью единой интеграции.
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: a3f5a2dc137a37012c4d7787d8c57c1045970be3
ms.sourcegitcommit: 31a9b4cb3d0f905f123475a4c1a86f5b1e59b935
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2020
ms.locfileid: "42219610"
---
# <a name="security-solution-integrations-using-the-microsoft-graph-security-api"></a>Интеграция решений по обеспечению безопасности с помощью Microsoft Graph Security API

К Microsoft Graph Security API можно подключиться с помощью следующих возможностей. Они позволяют работать с данными в едином формате в разных [поддерживаемых решениях поставщиков безопасности партнеров и Майкрософт](https://aka.ms/graphsecurityalerts) с помощью единой интеграции.

- **Непосредственное использование поддерживаемых вариантов интеграции**. См. [список поддерживаемых вариантов интеграции](https://docs.microsoft.com/graph/security-concept-overview#why-use-the-microsoft-graph-security-api), например написание кода для прямого подключения приложения, чтобы получать более подробные сведения. Используйте [примеры](https://aka.ms/graphsecurityapicode), чтобы приступить к работе.
- **Использование встроенной интеграции и соединителей, созданных партнерами Майкрософт**. Чтобы использовать эти возможности интеграции, ознакомьтесь с [решениями партнеров для Microsoft Graph Security API](https://aka.ms/graphsecuritypartnerships).  
- **Использование соединителей, созданных Майкрософт**. См. [список соединителей](https://aka.ms/graphsecuritysolutionsconnectors), которые можно использовать для подключения к API с помощью разных решений для служб SIEM (инциденты безопасности и управление), SOAR (реагирование системы безопасности и согласование), ITSM (отслеживание инцидентов и управление службой), отчетности и т. д.  

## <a name="list-of-connectors-from-microsoft"></a>Список соединителей от Майкрософт

| Тип решения | Имя | Соединитель | Объявление |
|:-----|:--------|:--------|:----------|
| SIEM |Splunk Enterprise и Splunk Cloud|[Надстройка Microsoft Graph Security API для Splunk](https://aka.ms/graphsecuritysplunkaddon) | [Запись блога](https://aka.ms/graphsecuritysplunkaddonblogpost)<br>[Запись блога о Splunk в облаке](https://aka.ms/graphsecuritysplunkcloudblogpost)|
| SOAR | Azure Logic Apps / Microsoft Flow | [Соединитель Microsoft Graph Security для Azure Logic Apps, Microsoft Flow и PowerApps](https://aka.ms/graphsecurityconnectors) | [Запись блога](https://aka.ms/graphsecurityconnectorsblogpost) |
| Автоматизация | Модуль PowerShell | [Модуль PowerShell Microsoft Graph Security](https://aka.ms/graphsecuritypowershellmodule) | [Запись блога](https://aka.ms/graphsecuritypowershellmodulepost) |
| Отчетность | Power BI | [Соединитель Microsoft Graph Security для Power BI](https://aka.ms/graphsecuritypowerbiconnectordoc) | [Запись блога](https://aka.ms/graphsecuritypowerbiconnectorblogpost) |

Ознакомьтесь с [возможностями партнерства](https://docs.microsoft.com/graph/security-partner-overview), если вы хотите поддерживать встроенную интеграцию в своем решении или стать поставщиком данных для Microsoft Graph Security API.
