---
title: тип перечисления Кэйсторажепровидероптион
description: Параметры импорта поставщика хранилища ключей (KSP).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b422443abcdb72cd76399ae9f2e0fea59bb6f34f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807114"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="c6013-103">тип перечисления Кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="c6013-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="c6013-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6013-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6013-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c6013-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6013-106">Параметры импорта поставщика хранилища ключей (KSP).</span><span class="sxs-lookup"><span data-stu-id="c6013-106">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="c6013-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="c6013-107">Members</span></span>
|<span data-ttu-id="c6013-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="c6013-108">Member</span></span>|<span data-ttu-id="c6013-109">Значение</span><span class="sxs-lookup"><span data-stu-id="c6013-109">Value</span></span>|<span data-ttu-id="c6013-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c6013-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6013-111">Усетпмкспосервисеусесофтварексп</span><span class="sxs-lookup"><span data-stu-id="c6013-111">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="c6013-112">нуль</span><span class="sxs-lookup"><span data-stu-id="c6013-112">0</span></span>|<span data-ttu-id="c6013-113">Импорт в KSP доверенного платформенного модуля (TPM), если он присутствует, в противном случае импортировать в KSP программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="c6013-113">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="c6013-114">Усетпмкспосервисефаил</span><span class="sxs-lookup"><span data-stu-id="c6013-114">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="c6013-115">1,1</span><span class="sxs-lookup"><span data-stu-id="c6013-115">1</span></span>|<span data-ttu-id="c6013-116">Импорт в KSP доверенного ПЛАТФОРМЕНного модуля (TPM), если он присутствует, в противном случае произойдет ошибка.</span><span class="sxs-lookup"><span data-stu-id="c6013-116">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="c6013-117">Усепасспортфорворккспосервисефаил</span><span class="sxs-lookup"><span data-stu-id="c6013-117">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="c6013-118">2</span><span class="sxs-lookup"><span data-stu-id="c6013-118">2</span></span>|<span data-ttu-id="c6013-119">Импорт в паспорт для Works KSP, если он доступен, в противном случае произойдет ошибка.</span><span class="sxs-lookup"><span data-stu-id="c6013-119">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="c6013-120">Усесофтварексп</span><span class="sxs-lookup"><span data-stu-id="c6013-120">useSoftwareKsp</span></span>|<span data-ttu-id="c6013-121">4</span><span class="sxs-lookup"><span data-stu-id="c6013-121">3</span></span>|<span data-ttu-id="c6013-122">Импорт в KSP программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="c6013-122">Import to Software KSP.</span></span>|





