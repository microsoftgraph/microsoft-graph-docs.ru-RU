---
title: тип перечисления Мобилеаппсуперседенцетипе
description: Указывает тип замены, связанный с отношением между двумя мобильными приложениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: aa947a2d5ad5b580de49180fee573a4f7d395952
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733289"
---
# <a name="mobileappsupersedencetype-enum-type"></a><span data-ttu-id="ef43d-103">тип перечисления Мобилеаппсуперседенцетипе</span><span class="sxs-lookup"><span data-stu-id="ef43d-103">mobileAppSupersedenceType enum type</span></span>

<span data-ttu-id="ef43d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef43d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef43d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef43d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef43d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef43d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef43d-107">Указывает тип замены, связанный с отношением между двумя мобильными приложениями.</span><span class="sxs-lookup"><span data-stu-id="ef43d-107">Indicates the supersedence type associated with a relationship between two mobile apps.</span></span>

## <a name="members"></a><span data-ttu-id="ef43d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ef43d-108">Members</span></span>
|<span data-ttu-id="ef43d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ef43d-109">Member</span></span>|<span data-ttu-id="ef43d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ef43d-110">Value</span></span>|<span data-ttu-id="ef43d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ef43d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef43d-112">исправления</span><span class="sxs-lookup"><span data-stu-id="ef43d-112">update</span></span>|<span data-ttu-id="ef43d-113">нуль</span><span class="sxs-lookup"><span data-stu-id="ef43d-113">0</span></span>|<span data-ttu-id="ef43d-114">Указывает, что дочернее приложение должно обновляться внутренней логикой родительского приложения.</span><span class="sxs-lookup"><span data-stu-id="ef43d-114">Indicates that the child app should be updated by the internal logic of the parent app.</span></span>|
|<span data-ttu-id="ef43d-115">replace</span><span class="sxs-lookup"><span data-stu-id="ef43d-115">replace</span></span>|<span data-ttu-id="ef43d-116">1,1</span><span class="sxs-lookup"><span data-stu-id="ef43d-116">1</span></span>|<span data-ttu-id="ef43d-117">Указывает, что дочернее приложение должно быть удалено перед установкой родительского приложения.</span><span class="sxs-lookup"><span data-stu-id="ef43d-117">Indicates that the child app should be uninstalled before installing the parent app.</span></span>|





