---
title: Тип ресурса Едукатионсинчронизатионконнектионсеттингс
description: 'Представляет параметры подключения к поставщику. Это позволяет системе узнать, как подключаться к API поставщика. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 449dc1c4265355d55e6d3ceb51fe86be9f84ac31
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979565"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a>Тип ресурса Едукатионсинчронизатионконнектионсеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры подключения к поставщику. Это позволяет системе узнать, как подключаться к API поставщика.

> [!NOTE]
> Этот сложный тип является абстрактным. Ознакомьтесь со списками определенных типов параметров подключения.

## <a name="derived-types"></a>Производные типы

| Тип                                                                                                                                      | Описание                                                                   |
| :---------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------- |
| [educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)                                   | Используйте этот тип для предоставления параметров подключения OAuth1.                          |
| [educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | Используйте этот тип для предоставления учетных данных клиента OAuth2 для предоставления параметров подключения. |

## <a name="properties"></a>Свойства

| Свойство     | Тип   | Описание                                                   |
| :----------- | :----- | :------------------------------------------------------------ |
| clientId     | String | Идентификатор клиента, используемый для подключения к поставщику.                    |
| clientSecret | String | Секрет клиента для проверки подлинности подключения к поставщику. |


