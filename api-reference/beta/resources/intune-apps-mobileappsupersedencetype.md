---
title: тип перечисления Мобилеаппсуперседенцетипе
description: Указывает тип замены, связанный с отношением между двумя мобильными приложениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f475d32aa8ef4427eada5a049e54c8f3a73e3018
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49217076"
---
# <a name="mobileappsupersedencetype-enum-type"></a><span data-ttu-id="ae47b-103">тип перечисления Мобилеаппсуперседенцетипе</span><span class="sxs-lookup"><span data-stu-id="ae47b-103">mobileAppSupersedenceType enum type</span></span>

<span data-ttu-id="ae47b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae47b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae47b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae47b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae47b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae47b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae47b-107">Указывает тип замены, связанный с отношением между двумя мобильными приложениями.</span><span class="sxs-lookup"><span data-stu-id="ae47b-107">Indicates the supersedence type associated with a relationship between two mobile apps.</span></span>

## <a name="members"></a><span data-ttu-id="ae47b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ae47b-108">Members</span></span>
|<span data-ttu-id="ae47b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ae47b-109">Member</span></span>|<span data-ttu-id="ae47b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ae47b-110">Value</span></span>|<span data-ttu-id="ae47b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ae47b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae47b-112">исправления</span><span class="sxs-lookup"><span data-stu-id="ae47b-112">update</span></span>|<span data-ttu-id="ae47b-113">нуль</span><span class="sxs-lookup"><span data-stu-id="ae47b-113">0</span></span>|<span data-ttu-id="ae47b-114">Указывает, что дочернее приложение должно обновляться внутренней логикой родительского приложения.</span><span class="sxs-lookup"><span data-stu-id="ae47b-114">Indicates that the child app should be updated by the internal logic of the parent app.</span></span>|
|<span data-ttu-id="ae47b-115">replace</span><span class="sxs-lookup"><span data-stu-id="ae47b-115">replace</span></span>|<span data-ttu-id="ae47b-116">1,1</span><span class="sxs-lookup"><span data-stu-id="ae47b-116">1</span></span>|<span data-ttu-id="ae47b-117">Указывает, что дочернее приложение должно быть удалено перед установкой родительского приложения.</span><span class="sxs-lookup"><span data-stu-id="ae47b-117">Indicates that the child app should be uninstalled before installing the parent app.</span></span>|




