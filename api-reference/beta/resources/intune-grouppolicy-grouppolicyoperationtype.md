---
title: тип перечисления Граупполициоператионтипе
description: Тип операции с групповой политикой.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 12b3fe1a39119c466d61af10a840139ae11c1009
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684752"
---
# <a name="grouppolicyoperationtype-enum-type"></a><span data-ttu-id="96ede-103">тип перечисления Граупполициоператионтипе</span><span class="sxs-lookup"><span data-stu-id="96ede-103">groupPolicyOperationType enum type</span></span>

<span data-ttu-id="96ede-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96ede-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96ede-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96ede-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96ede-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="96ede-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96ede-107">Тип операции с групповой политикой.</span><span class="sxs-lookup"><span data-stu-id="96ede-107">Type of Group Policy operation.</span></span>

## <a name="members"></a><span data-ttu-id="96ede-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="96ede-108">Members</span></span>
|<span data-ttu-id="96ede-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="96ede-109">Member</span></span>|<span data-ttu-id="96ede-110">Значение</span><span class="sxs-lookup"><span data-stu-id="96ede-110">Value</span></span>|<span data-ttu-id="96ede-111">Описание</span><span class="sxs-lookup"><span data-stu-id="96ede-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96ede-112">none</span><span class="sxs-lookup"><span data-stu-id="96ede-112">none</span></span>|<span data-ttu-id="96ede-113">нуль</span><span class="sxs-lookup"><span data-stu-id="96ede-113">0</span></span>|<span data-ttu-id="96ede-114">Групповая политика: недопустимый тип операции.</span><span class="sxs-lookup"><span data-stu-id="96ede-114">Group Policy invalid operation type.</span></span>|
|<span data-ttu-id="96ede-115">загрузку</span><span class="sxs-lookup"><span data-stu-id="96ede-115">upload</span></span>|<span data-ttu-id="96ede-116">1,1</span><span class="sxs-lookup"><span data-stu-id="96ede-116">1</span></span>|<span data-ttu-id="96ede-117">Тип операции отправки групповой политики.</span><span class="sxs-lookup"><span data-stu-id="96ede-117">Group Policy upload operation type.</span></span>|
|<span data-ttu-id="96ede-118">уплоадневверсион</span><span class="sxs-lookup"><span data-stu-id="96ede-118">uploadNewVersion</span></span>|<span data-ttu-id="96ede-119">2</span><span class="sxs-lookup"><span data-stu-id="96ede-119">2</span></span>|<span data-ttu-id="96ede-120">Отправка типа операции новой версии групповой политики.</span><span class="sxs-lookup"><span data-stu-id="96ede-120">Group Policy upload new version operation type.</span></span>|
|<span data-ttu-id="96ede-121">аддлангуажефилес</span><span class="sxs-lookup"><span data-stu-id="96ede-121">addLanguageFiles</span></span>|<span data-ttu-id="96ede-122">4</span><span class="sxs-lookup"><span data-stu-id="96ede-122">3</span></span>|<span data-ttu-id="96ede-123">Тип операции "Добавление файлов нового языка" групповой политики (ADML).</span><span class="sxs-lookup"><span data-stu-id="96ede-123">Group Policy add new language(ADML) files operation type.</span></span>|
|<span data-ttu-id="96ede-124">ремовелангуажефилес</span><span class="sxs-lookup"><span data-stu-id="96ede-124">removeLanguageFiles</span></span>|<span data-ttu-id="96ede-125">4 </span><span class="sxs-lookup"><span data-stu-id="96ede-125">4</span></span>|<span data-ttu-id="96ede-126">Тип операции удаления файлов на языке групповой политики (ADML).</span><span class="sxs-lookup"><span data-stu-id="96ede-126">Group Policy remove language(ADML) files operation type.</span></span>|
|<span data-ttu-id="96ede-127">упдателангуажефилес</span><span class="sxs-lookup"><span data-stu-id="96ede-127">updateLanguageFiles</span></span>|<span data-ttu-id="96ede-128">5 </span><span class="sxs-lookup"><span data-stu-id="96ede-128">5</span></span>|<span data-ttu-id="96ede-129">Тип операции для файлов на языке обновлений групповой политики (ADML).</span><span class="sxs-lookup"><span data-stu-id="96ede-129">Group Policy update language(ADML) files operation type.</span></span>|
|<span data-ttu-id="96ede-130">удалить</span><span class="sxs-lookup"><span data-stu-id="96ede-130">remove</span></span>|<span data-ttu-id="96ede-131">6 </span><span class="sxs-lookup"><span data-stu-id="96ede-131">6</span></span>|<span data-ttu-id="96ede-132">Групповая политика удалить отправленный тип операции с файлами.</span><span class="sxs-lookup"><span data-stu-id="96ede-132">Group Policy remove uploaded file operation type.</span></span>|





