---
title: тип enum windowsDefenderApplicationControlSupplementalPolicyStatuses
description: Значения enum для различных статусов развертывания дополнительных политик WindowsDefenderApplicationControl.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fe8ed534f64188691f8e4cfd8e26322291f0f821
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057196"
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
|success|1|Действует дополнительная политика WindowsDefenderApplicationControl.|
|tokenError|2|Дополнительная политика WindowsDefenderApplicationControl является структурно нормальной, но при авторизации маркера существует ошибка.|
|notAuthorizedByToken|3|Маркер не разрешает эту дополнительную политику WindowsDefenderApplicationControl.|
|policyNotFound|4 |Дополнительная политика WindowsDefenderApplicationControl не найдена.|



