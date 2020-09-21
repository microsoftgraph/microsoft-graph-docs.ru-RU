---
title: ресурс educationSynchronizationOAuth1ConnectionSettings
description: Когда OAuth1 используется для подключения к поставщику данных, этот тип параметров подключения следует использовать для настройки профиля.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a73876185469ab762a08f409028880a4f7234d45
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989635"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a><span data-ttu-id="e5b82-103">ресурс educationSynchronizationOAuth1ConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="e5b82-103">educationSynchronizationOAuth1ConnectionSettings resource</span></span>

<span data-ttu-id="e5b82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5b82-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5b82-105">Когда OAuth1 используется для подключения к поставщику данных, этот тип параметров подключения следует использовать для настройки профиля.</span><span class="sxs-lookup"><span data-stu-id="e5b82-105">When OAuth1 is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="e5b82-106">Производный от [едукатионсинчронизатионконнектионсеттингс].</span><span class="sxs-lookup"><span data-stu-id="e5b82-106">Derived from [educationSynchronizationConnectionSettings].</span></span>

## <a name="properties"></a><span data-ttu-id="e5b82-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5b82-107">Properties</span></span>

| <span data-ttu-id="e5b82-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5b82-108">Property</span></span>     | <span data-ttu-id="e5b82-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e5b82-109">Type</span></span>   | <span data-ttu-id="e5b82-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e5b82-110">Description</span></span>                                                                                                                |
| :----------- | :----- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e5b82-111">clientId</span><span class="sxs-lookup"><span data-stu-id="e5b82-111">clientId</span></span>     | <span data-ttu-id="e5b82-112">String</span><span class="sxs-lookup"><span data-stu-id="e5b82-112">String</span></span> | <span data-ttu-id="e5b82-113">Идентификатор клиента, используемый для подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="e5b82-113">Client ID used to connect to the provider.</span></span> <span data-ttu-id="e5b82-114">Наследуется от [едукатионсинчронизатионконнектионсеттингс].</span><span class="sxs-lookup"><span data-stu-id="e5b82-114">Inherited from [educationSynchronizationConnectionSettings].</span></span>                    |
| <span data-ttu-id="e5b82-115">clientSecret</span><span class="sxs-lookup"><span data-stu-id="e5b82-115">clientSecret</span></span> | <span data-ttu-id="e5b82-116">String</span><span class="sxs-lookup"><span data-stu-id="e5b82-116">String</span></span> | <span data-ttu-id="e5b82-117">Секрет клиента для проверки подлинности подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="e5b82-117">Client secret to authenticate the connection to the provider.</span></span> <span data-ttu-id="e5b82-118">Наследуется от [едукатионсинчронизатионконнектионсеттингс].</span><span class="sxs-lookup"><span data-stu-id="e5b82-118">Inherited from [educationSynchronizationConnectionSettings].</span></span> |

[едукатионсинчронизатионконнектионсеттингс]: educationsynchronizationconnectionsettings.md
[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md

## <a name="json-representation"></a><span data-ttu-id="e5b82-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e5b82-120">JSON representation</span></span>

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


