---
title: Тип ресурса educationIdentitySynchronizationConfiguration
description: Абстрактный базовый класс для всех школа данных профиля identity синхронизации конфигураций. Производные классы определите поведение синхронизации удостоверения. Ниже приведены производные типы.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 59dca28f82de0340aa289c6ea96ef5e252f60e85
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412907"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="a8cd3-105">Тип ресурса educationIdentitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8cd3-105">educationIdentitySynchronizationConfiguration resource type</span></span>

> <span data-ttu-id="a8cd3-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a8cd3-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8cd3-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8cd3-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8cd3-108">Абстрактный базовый класс для всех школа данных профиля identity синхронизации конфигураций.</span><span class="sxs-lookup"><span data-stu-id="a8cd3-108">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="a8cd3-109">Производные классы определите поведение синхронизации удостоверения.</span><span class="sxs-lookup"><span data-stu-id="a8cd3-109">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="a8cd3-110">Ниже приведены производные типы.</span><span class="sxs-lookup"><span data-stu-id="a8cd3-110">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="a8cd3-111">Производные типы</span><span class="sxs-lookup"><span data-stu-id="a8cd3-111">Derived types</span></span>
| <span data-ttu-id="a8cd3-112">Тип</span><span class="sxs-lookup"><span data-stu-id="a8cd3-112">Type</span></span> | <span data-ttu-id="a8cd3-113">Описание</span><span class="sxs-lookup"><span data-stu-id="a8cd3-113">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="a8cd3-114">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="a8cd3-114">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="a8cd3-115">Этот тип используется в соответствии с существующим учетным записям пользователей в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="a8cd3-115">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="a8cd3-116">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="a8cd3-116">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="a8cd3-117">Этот тип используется для создания новых учетных записей пользователей в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a8cd3-117">Use this type to create new user accounts in Azure AD.</span></span> |

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{
}
```
