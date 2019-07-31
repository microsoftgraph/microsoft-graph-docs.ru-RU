---
title: тип перечисления Кэйсторажепровидероптион
description: Параметры импорта поставщика хранилища ключей (KSP).
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e345e5c3b8490c15edd83fd4d7a4eb70e4be40d5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001042"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="3a7f3-103">тип перечисления Кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="3a7f3-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="3a7f3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a7f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a7f3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a7f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a7f3-106">Параметры импорта поставщика хранилища ключей (KSP).</span><span class="sxs-lookup"><span data-stu-id="3a7f3-106">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="3a7f3-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="3a7f3-107">Members</span></span>
|<span data-ttu-id="3a7f3-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="3a7f3-108">Member</span></span>|<span data-ttu-id="3a7f3-109">Значение</span><span class="sxs-lookup"><span data-stu-id="3a7f3-109">Value</span></span>|<span data-ttu-id="3a7f3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3a7f3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a7f3-111">Усетпмкспосервисеусесофтварексп</span><span class="sxs-lookup"><span data-stu-id="3a7f3-111">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="3a7f3-112">нуль</span><span class="sxs-lookup"><span data-stu-id="3a7f3-112">0</span></span>|<span data-ttu-id="3a7f3-113">Импорт в KSP доверенного платформенного модуля (TPM), если он присутствует, в противном случае импортировать в KSP программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="3a7f3-113">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="3a7f3-114">Усетпмкспосервисефаил</span><span class="sxs-lookup"><span data-stu-id="3a7f3-114">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="3a7f3-115">1,1</span><span class="sxs-lookup"><span data-stu-id="3a7f3-115">1</span></span>|<span data-ttu-id="3a7f3-116">Импорт в KSP доверенного платформенного модуля (TPM), если он присутствует, в противном случае произойдет ошибка.</span><span class="sxs-lookup"><span data-stu-id="3a7f3-116">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="3a7f3-117">Усепасспортфорворккспосервисефаил</span><span class="sxs-lookup"><span data-stu-id="3a7f3-117">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="3a7f3-118">2</span><span class="sxs-lookup"><span data-stu-id="3a7f3-118">2</span></span>|<span data-ttu-id="3a7f3-119">Импорт в паспорт для Works KSP, если он доступен, в противном случае произойдет ошибка.</span><span class="sxs-lookup"><span data-stu-id="3a7f3-119">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="3a7f3-120">Усесофтварексп</span><span class="sxs-lookup"><span data-stu-id="3a7f3-120">useSoftwareKsp</span></span>|<span data-ttu-id="3a7f3-121">4</span><span class="sxs-lookup"><span data-stu-id="3a7f3-121">3</span></span>|<span data-ttu-id="3a7f3-122">Импорт в KSP программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="3a7f3-122">Import to Software KSP.</span></span>|





