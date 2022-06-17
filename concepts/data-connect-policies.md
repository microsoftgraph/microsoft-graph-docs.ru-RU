---
title: Политики и выставление счетов для подключения к данным Microsoft Graph
description: Сведения о политиках Azure, поддерживаемых для приложения, созданного на основе данных Microsoft 365, и счета, связанного с используемой вами фабрикой данных Azure.
author: fercobo-msft
ms.localizationpriority: high
ms.prod: data-connect
ms.openlocfilehash: cf3942063936f2b26811251290c9c4a135dfd43e
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093985"
---
# <a name="microsoft-graph-data-connect-policies-and-billing"></a>Политики и выставление счетов для подключения к данным Microsoft Graph

Подключение к данным Microsoft Graph осуществляется с помощью [управляемых приложений Azure](/azure/managed-applications/overview). С их помощью вы можете создать и развернуть решения в среде Azure. С помощью управляемых приложений вы можете поддерживать определенные политики Azure, обеспечивая клиентам более высокий доверительный уровень и комфорт при использовании приложений.

## <a name="policies"></a>Политики

Управляемые приложения Azure, созданные на основе данных Microsoft 365, поддерживают следующие политики Azure:

- [Встроенные определения политики Azure для службы хранилища Azure](/azure/storage/common/policy-reference)
- [Введение в Azure Data Lake Storage 2-го поколения](/azure/storage/blobs/data-lake-storage-introduction)
- [Встроенные определения политики Azure для Azure Data Lake Storage 1-го поколения](/azure/data-lake-store/policy-reference)

> [!NOTE]
> Azure Data Lake Storage 1-го и 2-го поколения используют разные политики, поскольку Azure Data Lake Storage 2-го поколения реализует службу хранилища Azure.

После проверки состояния соответствия политике, выбранной во время публикации в Azure Marketplace, она применяется ко всем установленным экземплярам приложения. Все выбранные политики, которые соответствуют требованиям, отображаются для лиц, утверждающих данные, в рамках запроса данных. В случае нарушения соответствия политике происходит сбой в работе канала и прекращается извлечение данных.

## <a name="billing"></a>Выставление счетов

Счет связан с подпиской Azure Фабрики данных Azure, которую вы используете. Цена в этой новой модели выставления счетов зависит от количества объектов Microsoft Graph, к которым вы обращаетесь. Дополнительные сведения о выставлении счетов см. на странице [Цены](https://azure.microsoft.com/pricing/details/graph-data-connect/).

Объекты каталога, за которые не взимается плата:

- BasicDataSet_v0.User
- BasicDataSet_v0.MailboxSettings
- BasicDataSet_v0.Manager
- BasicDataSet_v0.DirectReport

## <a name="see-also"></a>См. также

- [Выбор и фильтрация пользователей](data-connect-filtering.md)
- [Вопросы и ответы о подключении к данным](data-connect-faq.md)
