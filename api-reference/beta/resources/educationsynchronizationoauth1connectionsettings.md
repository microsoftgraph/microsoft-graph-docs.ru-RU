---
title: ресурс educationSynchronizationOAuth1ConnectionSettings
description: Когда OAuth1 используется для подключения к поставщику данных, этот тип параметров подключения следует использовать для настройки профиля.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 525809121b07616c6eb5077f1b12d5b736586065
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434923"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a><span data-ttu-id="40277-103">ресурс educationSynchronizationOAuth1ConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="40277-103">educationSynchronizationOAuth1ConnectionSettings resource</span></span>

<span data-ttu-id="40277-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40277-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40277-105">Когда OAuth1 используется для подключения к поставщику данных, этот тип параметров подключения следует использовать для настройки профиля.</span><span class="sxs-lookup"><span data-stu-id="40277-105">When OAuth1 is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="40277-106">Производный от [едукатионсинчронизатионконнектионсеттингс].</span><span class="sxs-lookup"><span data-stu-id="40277-106">Derived from [educationSynchronizationConnectionSettings].</span></span>

## <a name="properties"></a><span data-ttu-id="40277-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="40277-107">Properties</span></span>

| <span data-ttu-id="40277-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="40277-108">Property</span></span>     | <span data-ttu-id="40277-109">Тип</span><span class="sxs-lookup"><span data-stu-id="40277-109">Type</span></span>   | <span data-ttu-id="40277-110">Описание</span><span class="sxs-lookup"><span data-stu-id="40277-110">Description</span></span>                                                                                                                |
| :----------- | :----- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="40277-111">clientId</span><span class="sxs-lookup"><span data-stu-id="40277-111">clientId</span></span>     | <span data-ttu-id="40277-112">String</span><span class="sxs-lookup"><span data-stu-id="40277-112">String</span></span> | <span data-ttu-id="40277-113">Идентификатор клиента, используемый для подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="40277-113">Client ID used to connect to the provider.</span></span> <span data-ttu-id="40277-114">Наследуется от [едукатионсинчронизатионконнектионсеттингс].</span><span class="sxs-lookup"><span data-stu-id="40277-114">Inherited from [educationSynchronizationConnectionSettings].</span></span>                    |
| <span data-ttu-id="40277-115">clientSecret</span><span class="sxs-lookup"><span data-stu-id="40277-115">clientSecret</span></span> | <span data-ttu-id="40277-116">String</span><span class="sxs-lookup"><span data-stu-id="40277-116">String</span></span> | <span data-ttu-id="40277-117">Секрет клиента для проверки подлинности подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="40277-117">Client secret to authenticate the connection to the provider.</span></span> <span data-ttu-id="40277-118">Наследуется от [едукатионсинчронизатионконнектионсеттингс].</span><span class="sxs-lookup"><span data-stu-id="40277-118">Inherited from [educationSynchronizationConnectionSettings].</span></span> |

[едукатионсинчронизатионконнектионсеттингс]: educationsynchronizationconnectionsettings.md
[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md

## <a name="json-representation"></a><span data-ttu-id="40277-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40277-120">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
  "clientId": "String",
  "clientSecret": "String"
}
```
