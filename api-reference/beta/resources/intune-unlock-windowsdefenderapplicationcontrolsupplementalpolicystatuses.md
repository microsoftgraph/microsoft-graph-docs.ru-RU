---
title: тип enum windowsDefenderApplicationControlSupplementalPolicyStatuses
description: Значения enum для различных статусов развертывания дополнительных политик WindowsDefenderApplicationControl.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 17a32097dcbc7f678823cb3fdb076166bf1f5353aa581bfa69f7de16565b0726
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54181057"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicystatuses-enum-type"></a>тип enum windowsDefenderApplicationControlSupplementalPolicyStatuses

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Значения enum для различных статусов развертывания дополнительных политик WindowsDefenderApplicationControl.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Состояние дополнительной политики WindowsDefenderApplicationControl неизвестно.|
|success|1 |Действует дополнительная политика WindowsDefenderApplicationControl.|
|tokenError|2|Дополнительная политика WindowsDefenderApplicationControl является структурно нормальной, но при авторизации маркера существует ошибка.|
|notAuthorizedByToken|3 |Маркер не разрешает эту дополнительную политику WindowsDefenderApplicationControl.|
|policyNotFound|4 |Дополнительная политика WindowsDefenderApplicationControl не найдена.|




